# Ex02 Django ORM Web Application
## Date: 17.10.2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2024-10-17 214234](https://github.com/user-attachments/assets/4b255d68-187a-4e60-b0c4-f170d131ad09)

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
## Developed by: DEVA DHARSHINI.I
## Reg.no: 212223240026
```
File: Models.py

from django.db import models
from django.contrib import admin

class Employee (models.Model):
    unique_number=models.CharField(max_length=20,primary_key=True)
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    job=models.CharField(max_length=100)

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('unique_number','name','age','email','job')

File: Admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin

admin.site.register(Employee,EmployeeAdmin)
```

## OUTPUT

![Screenshot 2024-10-17 214420](https://github.com/user-attachments/assets/32b808a6-a396-4419-9976-471fd3bcbda6)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
