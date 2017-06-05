# Django Tutorial

Following Django tutorial from [Django website](https://docs.djangoproject.com/en/1.11/intro/tutorial01/)

## Virtual Environment

Make virtual environment in root of the project with:
```
python3 -m venv virtual-env
```
Activate it with:
```
source virtual-env/bin/activate
```
Install Requirements with:
```
(virtual-env) ~/mysite$ python -m pip install -r requirements.txt
```

## Database setup
You need to be in **mysite** folder for this command:
```
(virtual-env) ~/mysite$ python manage.py migrate
```
To load initial data:
```
(virtual-env) ~/mysite$ python manage.py loaddata polls/fixtures/initial_data.json 
```
To dump your data to initial_data.json:
```
(virtual-env) ~/mysite$ python manage.py dumpdata polls > polls/fixtures/initial_data.json
```
## The development web server

You need to be in **mysite** folder for this command:
```
(virtual-env) ~/mysite$ python manage.py runserver
```

### Changing the port

By default, the runserver command starts the development server on the internal IP at port 8000.

If you want to change the server’s port, pass it as a command-line argument. For instance, this command starts the server on port 8080:
```
(virtual-env) ~/mysite$ python manage.py runserver 8080
```
If you want to change the server’s IP, pass it along with the port. For example, to listen on all available public IPs (which is useful if you are running Vagrant or want to show off your work on other computers on the network), use:
```
(virtual-env) ~/mysite$ python manage.py runserver 0:8000
```
**0** is a shortcut for **0.0.0.0**. Full docs for the development server can be found in the runserver reference.

## Django admin

Create superuser like this:

```
(virtual-env) ~/mysite$ python manage.py createsuperuser
Username: admin
Email address: admin@admin.com
Password:
Password (again):
Superuser created successfully.
```

After this you can use Django admin. Just go to the page **http://127.0.0.1:8000/admin/** and use credential you just entered.

