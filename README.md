#API for YaMdb
## Developers
    - Stas Zatushevskii

### .env
    DB_ENGINE=django.db.backends.postgresql # указываем, что работаем с postgresql

    DB_NAME=postgres # имя базы данных

    POSTGRES_USER=postgres # логин для подключения к базе данных

    POSTGRES_PASSWORD=postgres # пароль для подключения к БД (установите свой)

    DB_HOST=db # название сервиса (контейнера)

    DB_PORT=5432 # порт для подключения к БД 

### commands to run

1   __docker-compose up -d --build__

2   __docker-compose exec web python manage.py migrate__

3   __docker-compose exec web python manage.py createsuperuser__
    
4   __docker-compose exec web python manage.py collectstatic --no-input__