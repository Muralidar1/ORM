# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
from .models import Movie, MovieAdmin
admin.site.register(Movie,MovieAdmin)

models.py

from django.db import models
from django.contrib import admin
class Movie(models.Model):
    Mid=models.CharField(max_length=20,help_text="Movie ID")
    Name=models.CharField(max_length=10)
    Genre=models.CharField(max_length=20)
    Rating=models.IntegerField()
    Collection=models.IntegerField()
    YearofRelease=models.DateField()
    
class MovieAdmin(admin.ModelAdmin):
    list_display=('Mid','Name','Genre','Rating','Collection','YearofRelease')

```



## OUTPUT

![alt text](<Screenshot (5).png>)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
