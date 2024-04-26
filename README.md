# Homework "CRUD rest api methods"

Database development, administration and protection, College Sirius, Spring 2024

## Task

1. Сделать `create`/`read`/`update`/`delete` `rest api` методы на `flask` для указанной темы и сущности.
    - `read` метод должен так же возвращать связанные сущности в виде массива объектов.
    - в запросах к базе данных должна быть предусмотрена защита от SQL инъекций.

2. Раскатка базы данных должна производиться с помощью миграций.
    - базу данных и схему использовать отличные от дефолтных.
    - для id использовать тип `uuid`.

3. Запуск должен производиться через `docker compose`.
    - параметры запуска должны задаваться через `.env` файл.

## Topic and essence

Продукты и акции:
- на продукт может действовать несколько акций.
- акция может включать несколько продуктов.
- продукт - название, цена, категория.
- акция - название, размер скидки, дата начала, дата завершения.

Продукты и отзывы:
- продукт может иметь несколько отзывов.
- отзыв может принадлежать только одному продукту.
- отзыв - текст, оценка.

`CRUD` для продуктов.

### Environment variables
POSTGRES_HOST=<change_me>\
POSTGRES_PORT=<change_me>\
POSTGRES_DB=<change_me>\
POSTGRES_USER=<change_me>\
POSTGRES_PASSWORD=<change_me>

FLASK_PORT=<change_me>