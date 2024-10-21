# Ex02 Django ORM Web Application
## Date: 22.10.2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![Alt text](<Screenshot 2024-10-21 224846.png>)

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
models.py

from django.db import models
from django.contrib import admin
class Bank(models.Model):
         Name=models.CharField(max_length=10)
         Accountno=models.IntegerField(primary_key="accountno")
         Aadharno=models.IntegerField()
         DoB=models.DateField()
         Email=models.EmailField()
         Branch=models.CharField(max_length=21)
         Photo=models.ImageField()
class BankAdmin(admin.ModelAdmin):

         list_display=('Name','Accountno','Aadharno','DoB','Email','Branch','Photo')

admin.py

from django.contrib import admin
from.models import Bank,BankAdmin
admin.site.register(Bank,BankAdmin)
```

## OUTPUT

![Alt text](<Screenshot (1).png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
