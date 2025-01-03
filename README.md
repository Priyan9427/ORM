# Ex02 Django ORM Web Application
# Date:7/10/24
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM


![orm](https://github.com/user-attachments/assets/c07c84d9-f470-4518-aef9-92fa413a2ce5)



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

![Screenshot 2025-01-02 144207](https://github.com/user-attachments/assets/713e76e6-f301-41fe-9e1b-e03eac336b8d)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
