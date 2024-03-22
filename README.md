# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![mku](https://github.com/RITHISHlearn/ORM/assets/145446645/c177512c-1f3c-4471-97d9-f5082f79ff9f)
 


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
## Model.py:


from django.db import models

from django.contrib import admin

class Employee (models.Model):

    eid=models.CharField(max_length=20,help_text="Employee ID")
    
    name=models.CharField(max_length=100)
    
    salary=models.IntegerField()
    
    age=models.IntegerField()
    
    email=models.EmailField()
    
 
class EmployeeAdmin(admin.ModelAdmin):

    list_display=('eid','name','salary','age','email')
    

## Admin.py:


from django.contrib import admin

from .models import Employee,EmployeeAdmin

admin.site.register(Employee,EmployeeAdmin)

 

## OUTPUT

 ![mk](https://github.com/RITHISHlearn/ORM/assets/145446645/44e12460-e709-4853-a9aa-6635986fc7c4)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
