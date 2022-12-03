### Описание проекта:
Учебный проект, предназначенный для отработки навыков и применение теории при разработки
API веб приложений, базируемых на фреймворке Django и модуле Django Rest Framework.
Для обеспечения контороля прав доступа в проекте используется модуль Djoser.

### Установка и запуск проекта:

Клонировать репозиторий:
git clone https://github.com/shmyrev/api_final_yatube.git

Создать окружение:
python3 -m venv venv

Запуск окружения:
source venv/bin/activate

Установить зависимости:
pip install -r requirements.txt

Выполните миграцию:
python3 manage.py migrate

Запуск проекта:
python3 manage.py runserver

По адресу http://127.0.0.1:8000/redoc/ будет доступна документация для API

### Примеры запросов к API:
GET http://127.0.0.1:8000/api/v1/posts/
POST http://127.0.0.1:8000/api/v1/posts/
GET http://127.0.0.1:8000/api/v1/posts/{id}/
GET http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
POST http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
GET http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/
GET http://127.0.0.1:8000/api/v1/groups/
GET http://127.0.0.1:8000/api/v1/follow/
POST http://127.0.0.1:8000/api/v1/follow/