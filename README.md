# devspoon-django-basic-dev-env
this repositry is base frame for django development .

# How to use
## export mode

Development mode
1. enter command "export DJANGO_SETTINGS_MODULE=django_basic.settings.dev"
2. python manage.py makemigrations
3. python manage.py migrate
4. python manage.py runserver 0.0.0.0:8000

Product mode
1. enter command "export DJANGO_SETTINGS_MODULE=django_basic.settings.prod"
2. python manage.py makemigrations
3. python manage.py migrate
4. python manage.py runserver 0.0.0.0:8000

AWS mode
1. enter command "export DJANGO_SETTINGS_MODULE=django_basic.settings.fabfile"
2. python manage.py makemigrations
3. python manage.py migrate
4. python manage.py runserver 0.0.0.0:8000

## modify manage.py and wsgi.py mode
> manage.py and wsgi.py update like bellow

Development mode    
- os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'django_basic.settings.dev')    


Product mode
-  os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'django_basic.settings.prod')

AWS mode
- os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'django_basic.settings.fabfile')