# Creation Process for Creating this Website

## Initial Set Up

### Python

Currently using Python 3.10.7 in the virtual environment

### Django

Currently using django-admin 5.0

### Project Set Up

```console
$ django-admin startproject hknbe_main
```

### Create Apps

In the folder where the app should be stored:

```console
python manage.py startapp <name>
```

Then update:
- `views.py`: add any html and views
Added views to `views.py` and then update urls in `urls.py` and the urls in `hknbe_main/urls.py`.
Created `member_resources/templates` and update `settings.py` to see the new app. Updated it using:

```console
python manage.py migrate
```

### Adding Models

Add model to `models.py` then run:

```console
python manage.py makemigrations <name>
python manage.py migrate
```

To view SQL statements that were executed, use:

```console
python manage.py sqlmigrate <name> <migration_number>
```

## Development

### Testing

```console
$ python manage.py runserver
```
