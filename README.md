# Django Tutorial

Following Django tutorial from [Django website](https://docs.djangoproject.com/en/1.11/intro/tutorial01/)

## The development server

Change into the outer mysite directory, if you haven’t already, and run the following commands:
```
$ python manage.py runserver
```

### Changing the port

By default, the runserver command starts the development server on the internal IP at port 8000.

If you want to change the server’s port, pass it as a command-line argument. For instance, this command starts the server on port 8080:
```
$ python manage.py runserver 8080
```
If you want to change the server’s IP, pass it along with the port. For example, to listen on all available public IPs (which is useful if you are running Vagrant or want to show off your work on other computers on the network), use:
```
$ python manage.py runserver 0:8000
```
**0** is a shortcut for **0.0.0.0**. Full docs for the development server can be found in the runserver reference.

## Django admin

Admin credentials:

username: **admin**

password: **adminpassword**