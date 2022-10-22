# Docker yml setup for django, postgres, pgadmin

### GET STARTED

#### Git Clone
```
git clone https://github.com/pompy/django_postgres_pgadmin
```
#### Make sure docker, docker-compose is installed
Installations depends on whether your os is based on windows or linux distribution

#### Docker Compose Up

```
// This instructs Composer to run django-admin startproject myproj in a container, using the web service’s image and configuration.
docker-compose run web django-admin startproject myproj .

// create and start containers
docker-compose up

//Run http://127.0.0.1:8000/ for site
//Run http://127.0.0.1:5050/browser/ for pgadmin

```

#### Django installations & other commands in local for reference

```
python -m ensurepip
python -m pip install Django
git clone https://github.com/django/django.git
python -m pip install -e django/

django-admin startproject HelloWorld
python manage.py runserver

// installing requirements
pip install -r requirements.txt

//migrations
python manage.py makemigrations
python manage.py migrate

```
