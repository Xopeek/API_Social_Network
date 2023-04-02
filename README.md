# API социальной сети Yatube
# Описание:
 
Финальная и окончательная часть учебного проекта социальной сети, которая включается в себя множество возможностей (Опубликование записей, комментирование, система подписки\отписки и т.д.)

# Стек:
- Python 3.9
- Django 3.2.16
- Django Rest Framework
- Pytest
- Simple-JWT
- SQLite3

# Инструкция по установке проекта из репозитория (Linux и macOS)

1. Клонировать репозиторий и перейти в него в командной строке:
---
    git clone git@github.com:Xopeek/api_final_yatube.git
---
    cd API_YaTube


2. Cоздать и активировать виртуальное окружение:
---
    python3 -m venv env
---
    source env/bin/activate

3. Установить зависимости из файла requirements.txt:
---
    python3 -m pip install --upgrade pip
---
    pip install -r requirements.txt

4. Выполнить миграции:
---
    cd yatube_api
---
    python3 manage.py migrate

5. Запустить проект (в режиме сервера Django):
---
    python3 manage.py runserver

# Примеры запросов:
1. Получить список постов:
---
    GET /api/v1/posts/
2. Опубликовать новый пост:
---
    POST /api/v1/posts/
3. Получить список групп:
---
    GET /api/v1/groups/
4. Добавить коммент к посту:
---
    POST /api/v1/posts/{post_id}/comments/
5. Получить список подписок:
---
    GET /api/v1/follow/


# Документация к проекту
Документация для API после установки доступна по адресу /redoc/.




### Автор проекта Xopek -_- (Семляков Игорь)