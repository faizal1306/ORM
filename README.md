# Ex02 Django ORM Web Application
## Name: Moahmed Faizal M
## Date:

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
models.py
from django.db import models
from django.contrib import admin
class Movie(models.Model):
    USER_ID = models.CharField(max_length=300,help_text='USER ID')
    USER_NAME = models.CharField(max_length=300)
    PHONE_NUMBER = models.IntegerField()
    EMAIL = models.EmailField()
    MOVIE_NAME = models.CharField(max_length=300)
    DATE = models.DateField()
    SHOW_TIME = models.TimeField()
    SEATS_Number= models.IntegerField()

class MovieAdmin(admin.ModelAdmin):
    list_display = ('USER_ID', 'USER_NAME', 'PHONE_NUMBER', 'EMAIL', 'MOVIE_NAME', 'DATE','SEATS_Number','SHOW_TIME')

    admin.py
    from django.contrib import admin
from .models import Movie,MovieAdmin

admin.site.register(Movie,MovieAdmin)

```


## OUTPUT
<img width="1039" height="614" alt="Screenshot 2025-09-20 133011" src="https://github.com/user-attachments/assets/bb9a6b2e-4476-475e-bd20-3a520867ecf4" />




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
