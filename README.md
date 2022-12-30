# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve bus information using orm.

## Entity Relationship Diagram

### Bus Information Entity Diagram
![entity](https://user-images.githubusercontent.com/119560501/210038526-e7529b12-d979-4d6d-b165-a24bbb8f51ab.jpg)



## DESIGN STEPS

S### TEP 1:
Clone the repository to theia ide. start a new app inside the project folder.

### STEP 2:
Type the appropriate code for your table and provide appropriate data types to the columns.

### STEP 3:
Create a report about your project in readme.md file and upload the django.orm.app folder to your remote repository.
## PROGRAM
```

from django.db import models
from django.contrib import admin
# Create your models here.
class Bus(models.Model):
    Busno = models.IntegerField(primary_key=True, help_text="Busno")
    driver=models.CharField(max_length=100)
    From=models.CharField(max_length=100)
    To=models.CharField(max_length=100)
    noofseats=models.IntegerField()
class Businfo(admin.ModelAdmin):
    list_display = ('Busno','driver','From','To','noofseats')    

```

## OUTPUT
### BusInfo Table
![Django-orm](https://user-images.githubusercontent.com/119560501/210038645-7194e160-c31b-4357-b140-e19a4b633e9a.png)



## RESULT

Thus the project is developed to have Bus information database
