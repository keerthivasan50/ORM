# Ex02 Django ORM Web Application
## Date: 28.02.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![WhatsApp Image 2024-04-24 at 09 20 19_d38eebf7](https://github.com/keerthivasan50/ORM/assets/150429883/a80950e9-d4a2-4965-9510-69daaf052c2d)



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
from .models import book_DB,book_DBAdmin
admin.site.register(book_DB,book_DBAdmin)

models.py
from django.db import models
from django.contrib import admin
class Book_dbs(models.Model):
    bookno=models.IntegerField(primary_key=True);
    bookname=models.CharField(max_length=10);
    authorname=models.CharField(max_length=10);
    yearofpublishing=models.DateField();
    pages=models.IntegerField();
    price=models.IntegerField();

class book_DBAdmin(admin.ModelAdmin):
   list_display=("bookno","bookname","authorname","yearofpublishing","pages","price");
```


## OUTPUT
![WhatsApp Image 2024-04-24 at 09 20 19_d4199072](https://github.com/keerthivasan50/ORM/assets/150429883/2bbbaaa3-5417-4215-abfc-965d8ff6e521)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
