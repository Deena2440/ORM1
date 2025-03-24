# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/ce32f6b6-2536-42e7-b999-5230cdebe4dc)
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
```css
models.py

from django.db import models                                                                                                                      
from django.contrib import admin                                             
class book(models.Model):                    				      
   bookno=models.IntegerField(primary_key=True);                                                      
   authorname=models.CharField(max_length=50);                                                            
   price=models.IntegerField(help_text="enter price");                       
   qty=models.IntegerField();                                                
   bookname=models.CharField(max_length=50);                                 
class bookAdmin(admin.ModelAdmin):                                           
   list_display=("bookno","authorname","price","qty","bookname"); 

admin.py

from django.contrib import admin                                             
from .models import book,bookAdmin                                           
admin.site.register(book,bookAdmin)
```
# OUTPUT
Include the screenshot of your admin page.

![image](https://github.com/user-attachments/assets/038b2f9c-9ce6-4b88-821a-c8a7a6a72ae0)
![image](https://github.com/user-attachments/assets/a08aa7a8-819b-4771-9380-7373289e033e)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
