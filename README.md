# Проект Kittygram
### Проект позволяет делиться своими котиками, их фотографиями, достижениями.
### Загрузить фотографию своего котика, при необходимости удалить либо изменить о нем информацию

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone git@github.com:AndreyYP/kittygram_final.git
```

```
cd kittygram
```

Cоздать и активировать виртуальное окружение:

```
py -m venv env
```

```
source venv/Scripts/activate
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
py manage.py migrate
```

Запустить проект череp docker compose :

```
docker compose up --build
```
```
docker compose exec backend python manage.py collectstatic
```
```
docker compose exec backend cp -r /app/collected_static/. /backend_static/static/
```
Сайт доступен по адресу - http://127.0.0.1:9000/