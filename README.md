# Ex02 Django ORM Web Application
# Date:27/11/2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).


## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
model.py
from django.db import models
from django.contrib import admin
class Bankloan (models.Model):
     acc=models.IntegerField(primary_key="acc")
     name=models.CharField(max_length=100)
     mobileno=models.IntegerField()
     pancode=models.IntegerField()
     aadharcode=models.IntegerField()
     
class BankloanAdmin(admin.ModelAdmin):
  list_display=('acc','name','mobileno','pancode','aadharcode')

admin.py
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)

 ```

# OUTPUT
Include the screenshot of your admin page.
![Screenshot 2024-12-02 052619](https://github.com/user-attachments/assets/417c9ce7-f807-4877-8dc2-dac8413bdffd)

![alt text](<Screenshot 2024-11-27 182713.png>)
# RESULT
Thus the program for creating a database using ORM hass been executed successfully
