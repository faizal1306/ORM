# Ex02 Django ORM Web Application
## Date: 26/9/24

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2024-09-28 083239](https://github.com/user-attachments/assets/0e879abe-9cdb-4182-95b1-ea34266c18d4)



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM:

admin.py
```
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```
models.py
```
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')


```



## OUTPUT
![Screenshot 2024-09-26 203116](https://github.com/user-attachments/assets/16166afc-7dc4-442f-b923-d12d7761b942)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
