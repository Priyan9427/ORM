# Ex02 Django ORM Web Application
# Date:16/12/24
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM


![diagram](https://github.com/user-attachments/assets/15b0f061-29ee-41b1-9cc5-7c95173e399b)


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
admin.py
from django.contrib import admin
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin)



models.py
from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    Name=models.CharField(max_length=100)
    Accountno=models.IntegerField(primary_key="Accountno")
    Startdate=models.DateField()
    Email=models.EmailField()
    Mobilenumber=models.IntegerField()
    Amount=models.IntegerField()

class bankloanAdmin(admin.ModelAdmin):
    list_display=('Name','Accountno','Startdate','Email','Mobilenumber','Amount')



```


# OUTPUT


![alt text](<Screenshot 2024-12-08 004726.png>)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
