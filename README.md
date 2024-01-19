Инструкция по установке:

* Клонировать репозиторий командой git clone <адрес репозитария>.
* Установить и активировать виртуальное окружение.
    python -m venv venv
    venv\Sripts\activate
* Создать БД (postgresql), выполнить миграции
    python manage.py migrate
* Создать superuser
    python manage.py createsuperuser
* Загрузить json-файлы расположеные в fixtures/goods:
    python manage.py loaddata fixtures/goods/categories.json
    python manage.py loaddata fixtures/goods/products.json 
* Запустить проект 
    python manage.py runserver