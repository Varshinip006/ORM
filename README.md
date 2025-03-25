# Ex02 Django ORM Web Application
# Date:25.03.2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![loan er](https://github.com/user-attachments/assets/8ffb446c-83ab-4f4a-adbf-89fe3f8f2ec7)

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
models.py

from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    customer_name=models.CharField(max_length=100,primary_key=True)
    customer_id=models.CharField(max_length=100)
    loan_no=models.IntegerField()
    loan_amount=models.IntegerField()
    email=models.EmailField()
 
class userAdmin(admin.ModelAdmin):
    list_display=('customer_name','customer_id','loan_no','loan_amount','email')

admin.py

from django.contrib import admin
from .models import bankloan,userAdmin
admin.site.register(bankloan,userAdmin)

```

# OUTPUT
Include the screenshot of your admin page.

![Screenshot (44)](https://github.com/user-attachments/assets/f66fcb5f-c9cc-4918-ac91-3ef310a33870)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
