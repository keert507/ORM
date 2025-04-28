# Ex02 Django ORM Web Application
## Date: 28.04.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![WhatsApp Image 2025-04-28 at 21 04 07_3bc54683](https://github.com/user-attachments/assets/35209927-c133-47bb-97d0-42305f20dfdc)



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
from .models import BankLoan,BankLoanAdmin
admin.site.register(BankLoan,BankLoanAdmin)
```
```
models.py

from django.db import models
from django.contrib import admin 
class BankLoan(models.Model):
  acc=models.IntegerField(primary_key="accno")
  ph=models.IntegerField()
  ifsc=models.CharField(max_length=100)
  loanno=models.IntegerField()
  adress=models.CharField(max_length=100)
  pan=models.IntegerField()
  adhar=models.IntegerField()

class BankLoanAdmin(admin.ModelAdmin):
 list_display=('acc','ph','ifsc','loanno','adress','pan','adhar',)
```

## OUTPUT

![WhatsApp Image 2025-04-28 at 21 05 16_95c429a6](https://github.com/user-attachments/assets/69e381c9-abea-4599-9629-09f48e0e2575)

![WhatsApp Image 2025-04-28 at 21 06 50_49e5d77c](https://github.com/user-attachments/assets/8f14d879-570a-45dc-98cd-dbb76f184e09)



## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
