# Ex02 Django ORM Web Application
## Date: 07.10.2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```
Admin.py

from django.contrib import admin
from .models import footballplayers,playersAdmin
admin.site.register(footballplayers,playersAdmin)

Models.py

from django.db import models
from django.contrib import admin
class footballplayers (models.Model):
    name=models.CharField(max_length=100)
    field=models.IntegerField()
    age=models.IntegerField()
    record=models.IntegerField()

class playersAdmin(admin.ModelAdmin):
    list_display=('name','field','age','record')

```

## OUTPUT

![Screenshot 2023-10-27 143920](https://github.com/Kamali22004796/ORM/assets/120567837/dc606b35-07d7-457e-90ca-6687e4a8e362)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully.
