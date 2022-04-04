# install

1. `pyenv local 3.10.3`
2. `python3 -m venv .venv`
3. `source .venv/bin/activate`
4. `python -m pip install --upgrade pip && pip install pip-tools`
5. `pip-sync requirements.txt dev_requirements.txt`

## how to add deps

1. add to requirements.in with or without version
2. run `pip-compile` or for dev `pip-compile dev_requirements.in`
3. add version to requirements.in if omitted in 1.
4. run `pip-sync` or for dev `pip-sync requirements.txt dev_requirements.txt`

## useful commands

project init `django-admin startproject django_project . `

app init `python manage.py startapp books`

add new migrations `python manage.py makemigrations books`

exec migrate `python manage.py migrate`

create su `python manage.py createsuperuser`

test `python manage.py test`

run `python manage.py runserver`

`python manage.py collectstatic`
