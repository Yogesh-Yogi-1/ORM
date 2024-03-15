# Ex02 Django ORM Web Application
## Date: 
12/03/2024
## AIM
To develop a Django application to store and retrieve data from a Railway database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-03-15 090052](https://github.com/Yogesh-Yogi-1/ORM/assets/148514598/321da8de-0954-46de-8a58-a5f4c12d0387)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 records

## PROGRAM
```
model.py

from django.db import models
from django.contrib import admin
class Railway_db(models.Model):
    trainno=models.IntegerField(primary_key=True);
    trainname=models.CharField(max_length=20);
    departure=models.CharField(max_length=50);
    arrival=models.CharField(max_length=50);
    distance=models.IntegerField();
class Railway_dbAdmin(admin.ModelAdmin):
    list_display=("trainno","trainname","departure","arrival","distance");

admin.py

from django.contrib import admin
from .models import Railway_db,Railway_dbAdmin
admin.site.register(Railway_db,Railway_dbAdmin)
```
## OUTPUT

![Screenshot 2024-03-14 224641](https://github.com/Yogesh-Yogi-1/ORM/assets/148514598/ddfd4a50-ef19-434e-921c-a8049229e2bb)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
