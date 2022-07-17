# api_final_yatube является инструментом для взаимодействия с сайтом Yatube через API.

![This is an image](https://i.ytimg.com/vi/5YJ_dlM1ibc/maxresdefault.jpg)
## Настройка и запуск:

***1)Клонируем репозиторий:***
``` 
• git clone git@github.com:PashkaVRN/api_final_yatube.git
``` 

***2)Создаём и активируем виртуальное окружение:***
``` 
• python -m venv venv
• source venv/Scripts/activate
``` 

***3)Устанавливаем зависимости:***
``` 
• pip install -r requirements.txt
``` 

***4)Создаём и применяем миграции:***
``` 
• python manage.py makemigrations
• python manage.py migrate
``` 
***5)Запускаем DEV сервера:***
``` 
• python manage.py runserver
``` 
***Технологии:***
``` 
• Django 2.2.16
• Python 3.9
• Djangorestframework 3.12.4
``` 
## Примеры запросов/ответов:
***GET /api/v1/posts/***
``` 
Response:
{
    "id": 0,
    "author": "alex",
    "text": "text_post",
    "pub_date": "2022-04-12T15:03:22Z",
    "image": "image",
    "group": 0
}
``` 
***POST /api/v1/posts/***
``` 
Request:
{
    "text": "some_text",
    "image": "pic",
    "group": 1
}
``` 
``` 
Response:
{
    "id": 0,
    "author": "username",
    "text": "some_text",
    "pub_date": "2022-04-12T15:17:10Z",
    "image": "pic",
    "group": 1
}
``` 
Более подробное описание API можно получить по адресу:
http://localhost:8000/redoc/
