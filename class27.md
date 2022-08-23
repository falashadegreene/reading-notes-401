# Django Models

## Using Models

Models are used to create the structure of stored data. When models are created you should define separate models for every object. From there Django can help with defining the relationship:

- `OneToOneField`
- `ForeignKey`
- `ManyToManyField`

When defining a Model it can be defined in a application's models.py file and they can be used as sub-classes of django.db.models.Model. See example below: 

`from django.db import models
from django.contrib.auth.models import User`


`class Board(models.Model):
    name = models.CharField(max_length=30, unique=True)
    description = models.CharField(max_length=100)`


`class Topic(models.Model):
    subject = models.CharField(max_length=255)
    last_updated = models.DateTimeField(auto_now_add=True)
    board = models.ForeignKey(Board, related_name='topics')
    starter = models.ForeignKey(User, related_name='topics')`


`class Post(models.Model):
    message = models.TextField(max_length=4000)
    topic = models.ForeignKey(Topic, related_name='posts')
    created_at = models.DateTimeField(auto_now_add=True)
    updated_at = models.DateTimeField(null=True)
    created_by = models.ForeignKey(User, related_name='posts')
    updated_by = models.ForeignKey(User, null=True, related_name='+')`

## commen feild arguments

- help text
- verbose names
- default 
- null 
- blank
- choices
- primary key 

## commen feild Types

- Charfield 
- TextField 
- Integerfield 
- Eamilfield
- autofield 
- foreignkey
- manytomanyfield

## Djang Admin

The purpose for admin is to help build a site that can allow you to view, update, and delete records. It can also be used to help with internal data management. To add models to admin application you first need register models and create a superuser.


## Things I would like to know more about


