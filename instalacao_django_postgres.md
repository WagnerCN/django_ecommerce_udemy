pip install django
djando-admin startproject <name_project> .
pip freeze > requirements.txt
pip install -r requirements.txt

# Sonfigurar setitings.py
DATABASES = {
    "default": {
        "ENGINE": "django.db.backends.postgresql",
        "NAME": "postgres",
        "USER": "postgres",
        "PASSWORD": "postgres",
        "HOST": "db",
        "PORT": 5432,
    }
}