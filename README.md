# Ex01 Django ORM Web Application
## Date:30.11.2025

## AIM
To develop a Django application to store and retrieve data from a customer Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 2 customer

## PROGRAM
 ```
model.py
from django.db import models
from django.contrib import admin
# Create your models here.
class Customer(models.Model):
    Customer_name = models.CharField(max_length=20, help_text="Enter Customer Name")
    age = models.IntegerField(help_text="Enter age between 18 to 22")
    dob = models.DateField()
    Customer_id = models.IntegerField(help_text="Enter the Register Number")

class CustomerAdmin(admin.ModelAdmin):
    list_display = ['Customer_name', 'age', 'dob', 'Customer_id']
Admin.py
from django.contrib import admin
from .models import Customer, CustomerAdmin
# Register your models here.
admin.site.register(Customer, CustomerAdmin)

```
## OUTPUT

 <img width="1901" height="800" alt="Screenshot 2025-11-30 140217" src="https://github.com/user-attachments/assets/7a5853d0-ca64-44b4-9e29-f1557aa55d4c" />


## RESULT
Thus the program for creating customer inventory database database using ORM hass been executed successfully
