# api_yamdb
**API YaMDB** - это проект, который предоставляет REST API для работы с базой данных отзывов на фильмы, книги и музыку. В этой базе данных пользователи могут оставлять отзывы и комментарии, а также ставить оценки произведениям.

### Технологии
Python 3.9
Django 3.2.16
DRF 3.12.4

### Запуск проекта в dev-режиме
- Установите и активируйте виртуальное окружение
- Установите зависимости из файла requirements.txt
```
pip install -r requirements.txt
``` 
- В папке с файлом manage.py:
Выполните миграцию БД и наполнение БД тестовыми данными:
```
python3 manage.py migrate
python3 manage.py load_csv_data
```
- Запустите приложение:
```
python3 manage.py runserver
```

- Протестируйте один из следующих запросов
```
http://127.0.0.1:8000/api/v1/auth/signup/
http://127.0.0.1:8000/api/v1/auth/token/
http://127.0.0.1:8000/api/v1/users/me/
```

### Авторы
- Геннадий Умикашвили: [github](https://github.com/Gennady-Umikashvili)
- Анатолий Шерин: [github](https://github.com/AnatoliyPracticum)
- Константин Волков : [github](https://github.com/tr202)
