# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM
```py
from django.db import models
from django.contrib import admin
# Create your models here.

class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    phone=models.IntegerField()
    

class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','phone')
```
```py
from django.contrib import admin
from .models import Student,StudentAdmin
# Register your models here.
admin.site.register(Student,StudentAdmin)
```



## OUTPUT

### serveroutput:
![serveroutput](serverout.png)

### clientoutput:
![clientoutput](studentlist.png)

### primarykey:
![primarykey](primarykey.png)



## RESULT
Program executed sucessfully
