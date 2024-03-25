# Ex02 Django ORM Web Application
## Date: 28.02.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![313469473-c1e8d53b-1640-4346-9f10-b5b0919eb9021](https://github.com/Hemaprasad-N/ORM/assets/135933397/0771166d-dd62-467b-8f27-828a1bbca753)




Include your ER diagram here

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
![image](https://github.com/Hemaprasad-N/ORM/assets/135933397/0d584fac-d69e-40c1-ae4b-5b56683c3b40)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
