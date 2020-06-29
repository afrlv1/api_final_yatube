**Реализация API на базе Django Rest Framework**
Для запуска проекта необходимо:
Установить зависимости:
_pip install -r requirements.txt_

Создать модели:
_python manage.py makemigrations_

Провести миграцию:
_python manage.py migrate_

Запустить сервер командой:
_python manage.py runserver_

Доступные методы:
_/api/v1/posts/ (GET, POST, PUT, PATCH, DELETE)

/api/v1/posts/<id> (GET, POST, PUT, PATCH, DELETE)

/api/v1/posts/<id>/comments (GET, POST, PUT, PATCH, DELETE)

/api/v1/posts/<id>/comments/<id> (GET, POST, PUT, PATCH, DELETE)

/api/v1/group/ (GET, POST)

/api/v1/follow/ (GET, POST)_

Для доступа к API необходимо получить токен:
Для этого создать POST-запрос 
l*ocalhost:8000/api/v1/token/* 
передав поля username и password. 
API вернет токен.