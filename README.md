# CRM_E-commerce-shop
# How to run

## Starting: Run the server & SQLite

The fastest way to run the bot is to run it in polling mode using SQLite database without all Celery workers for background jobs. This should be enough for quickstart:

``` bash
git clone https://github.com/iMshaLch/CRM_E-commerce-shop
cd CRM_E-commerce-shop/myshop
```

Create virtual environment (optional)
``` bash
python3 -m venv venv
source venv/bin/activate
```

Install all requirements:
```
pip install -r requirements.txt
```


Run migrations to setup SQLite database:
``` bash
python manage.py migrate
```

Create superuser to get access to admin panel:
``` bash
python manage.py createsuperuser
```

Write commant to run the server:
``` bash
python manage.py runserver
```

