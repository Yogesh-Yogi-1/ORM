# Ex02 Django ORM Web Application
## Date: 
12/03/2024
## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-03-12 211903](https://github.com/Yogesh-Yogi-1/ORM/assets/148514598/8a12428d-0d0d-4759-a19d-7124048b785d)


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
model.py

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
    bookno=models.IntegerField(primary_key=True);
    authorname=models.CharField(max_length=20);
    bookname=models.CharField(max_length=50);
    version=models.IntegerField();
    pageno=models.IntegerField();
class Book_DBAdmin(admin.ModelAdmin):
    list_display=("bookno","authorname","bookname","version","pageno");

admin.py

from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```
## OUTPUT

![Screenshot 2024-03-12 220539](https://github.com/Yogesh-Yogi-1/ORM/assets/148514598/627f9f1f-db5e-44d6-a0c4-88a3f6d6b9a8)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
