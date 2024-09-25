# Ex02 Django ORM Web Application
# Name: NIHIL KK
# REG NO: 212221223003
## Date:18/09/2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

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
Models.py

from django.db import models
from django.contrib import admin
class Players(models.Model):
    jrsy=models.CharField(max_length=20,help_text="Player Jrsy")
    name=models.CharField(max_length=100)
    cntry=models.CharField(max_length=100)
    age=models.IntegerField()
    height=models.IntegerField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('jrsy','name','cntry','age','height')


Admin.py

from django.contrib import admin
from .models import Players,EmployeeAdmin
admin.site.register(Players,EmployeeAdmin)
```


## OUTPUT

![281349897-94c3d887-112e-4b9b-b83a-7365148fb61f](https://github.com/user-attachments/assets/9fa0d352-e650-4ac2-a4c1-8c32aa7cade8)
![281349536-b2e404af-f088-492e-b606-6ebffece8f02](https://github.com/user-attachments/assets/41b7fa68-1c6b-4aa9-b93d-bf131e988ec9)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
