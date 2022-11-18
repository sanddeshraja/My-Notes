
to make non static websites

GET is a request  sent to server

### http status code

200 - ok
301 - Moved Permannently
403 - Forbidden
404 - Not Found
500 - Internal Server Error

pip3 install Django
django-admin startproject <project-name> 

 Python manage. py runserver.
python manage.py startapp hello

in view

def index(request):
  return HttpResponse("Hello,world")