# The Air Class Project : Server

## Project setup
```
virtualenv env
.\env\Scripts\activate  (for window os)
source env/bin/activate (for max && linux os)
pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py createadminuser

```

[comment]: <> (test comment)
<!---

### CollectStatic (for production)
```
python production.py makemigrations
python production.py migrate
python production.py collectstatic
```

-->
### Run Server
```
python manage.py runserver

```
[comment]: <> (python manage.py runsslserver 0.0.0.0:8000)

### Custom Command 
 - python mange.py clear_migration_files : delete all migration file in project.
 - python manage.py createadminuser : create super admin .
 - python manage.py delete_db_sqlite : delete db.sqlite3 if exists .
 - python manage.py project_reset : run -> clear_migration_files, delete_db_sqlite commands.
 - python manage.py project_refresh : run -> project_reset, makemigrations, migrate commands 
  

## login SuperUser
SuperUser was created in createadminuser process.
```
username  : admin
password : password
``` 


 
### Documents
[Django](https://docs.djangoproject.com/en/3.0/).  
[Django rest-framework](https://www.django-rest-framework.org/).
