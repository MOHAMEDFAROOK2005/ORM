# Ex02 Django ORM Web Application
## Date: 08-09-2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```

admin.py

from django.contrib import admin
from .models import Movies,MoviesAdmin
admin.site.register(Movies,MoviesAdmin)


models.py

from django.db import models
from django.contrib import admin
class Movies(models.Model):
    userid=models.IntegerField(primary_key=True)
    username=models.CharField(max_length=30)
    mobileno=models.IntegerField()
    mailid=models.EmailField()
    moviename=models.CharField(max_length=50)
    noofseats=models.IntegerField()
    date=models.DateField()

class MoviesAdmin(admin.ModelAdmin):
    list_display=('username','moviename','noofseats','mailid')


```



## OUTPUT

![Screenshot 2025-03-29 161737](https://github.com/user-attachments/assets/f74ee815-0ecc-44aa-b152-579c867e02a7)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
