# Ex02 Django ORM Web Application
## Date: 19-10-2024
## NAME: MOHAMED FAIZAL
## REGISTER NO: 24000006

## AIM
To develop a Django application to store and retrieve data from a Bank database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-10-03 114132 (1)](https://github.com/user-attachments/assets/9621fda5-b676-4698-afbc-84e8eea43c5c)



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 customers.

## PROGRAM

admin.py:
```
from django.contrib import admin
from .models import Bankloan, BankloanAdmin  
admin.site.register(Bankloan, BankloanAdmin)
```
models.py:
```
from django.db import models
from django.contrib import admin
from django.db import models
from django.contrib import admin

class Bankloan(models.Model):
    customerid= models.IntegerField(primary_key=True)
    customerrate = models.IntegerField()
    age = models.IntegerField()  
    cust_no = models.IntegerField()
    customerloan_purpose =models.CharField(max_length=500)

class BankloanAdmin(admin.ModelAdmin):
    list_display = ('customerid', 'customerrate', 'age', 'cust_no', 'customerloan_purpose')
```

## OUTPUT


![BANK IMG](https://github.com/user-attachments/assets/ecf232e6-84ac-40d1-9b7e-ade1cdde3bfb)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully

