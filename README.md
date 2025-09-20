# Ex02 Django ORM Web Application
## Date: 19.09.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).



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
from .models import Car_DB,Car_DBAdmin
admin.site.register (Car_DB,Car_DBAdmin)

models.py


from django.db import models
from django.contrib import admin
class Car_DB(models.Model):
    Brand_Name = models.CharField(max_length=10)
    Model_No = models.IntegerField(primary_key=True)
    Customer_name = models.CharField(max_length=10)
    Mfg_Date = models.DateField()
class Car_DBAdmin(admin.ModelAdmin):
    list_display = ["Brand_Name","Model_No","Customer_name","Mfg_Date"]
```


## OUTPUT
![alt text](<Screenshot 2025-09-20 150904.png>)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
