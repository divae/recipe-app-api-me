# Recipe App API

Source code for my Udemy course Build a [Backend REST API with Python & Django - Advanced](http://udemy.com/django-python-advanced/).

The course teaches how to build a fully functioning REST API using:

 - Python
 - Django / Django-REST-Framework
 - Docker / Docker-Compose
 - Test Driven Development

## Getting started

To start project, run:

```
docker-compose up
```

*remember create super user the first time
```
docker-compose run app sh -c "python manage.py createsuperuser"
```

The API will then be available at http://127.0.0.1:8000

## Make migrations
```
docker-compose run app sh -c "python manage.py makemigrations `modulename`"
```

## Test

To run test :
```
docker-compose run app sh -c "python manage.py test && flake8"
```