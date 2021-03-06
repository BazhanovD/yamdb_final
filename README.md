# REST API для проекта YaMDb
[![Actions Status](https://github.com/BazhanovD/yamdb_final/workflows/Yamdb_final/badge.svg)](https://github.com/BazhanovD/yamdb_final/actions)

Проект YaMDb создан для хранения отзывов пользователей на различные произведения из категорий "Книги" и "Фильмы". Список категорий может быть расширен (можно, к примеру, добавить категорию "Музыка"). Произведению может быть присвоен жанр из списка предустановленных (например, "Сказка", "Хоррор" или "Боевик"). Пользователи выставляют произведению оценку по десятибалльной шкале. По их оценкам выставляется средний рейтинг произведения.

# Установка
Клонируйте репозиторий.
```
git clone https://github.com/BazhanovD/yamdb_final
```
Команда для запуска терминала внутри контейнера:
```
docker-compose exec web bash
```
Чтобы сделать миграцию бд, выполните следующую команду:
```
python manage.py migrate
```
Для создания администратора Django:
```
python manage.py createsuperuser
```
Чтобы загрузить в БД тестовые данные, выполните:
```
python manage.py loaddata fixtures.json
```
Команда для остановки контейнеров:
```
docker-compose down
```
Команда для повторного запуска:
```
docker-compose up -d
```

