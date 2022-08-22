
# What is Django

Django is a high-level Python web framework that enables rapid development of secure and maintainable websites. (credit: https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction#what_does_django_code_look_like)

Django includes dozens of extras you can use to handle common web development tasks. Django takes care of user authentication, content administration, site maps, RSS feeds, and many more tasks — right out of the box. (credit: https://www.djangoproject.com/start/overview/)

## Object-relational mapper

class Band(models.Model):
    """A model of a rock band."""
    name = models.CharField(max_length=200)
    can_rock = models.BooleanField(default=True)


class Member(models.Model):
    """A model of a rock band member."""
    name = models.CharField("Member's name", max_length=200)
    instrument = models.CharField(choices=(
            ('g', "Guitar"),
            ('b', "Bass"),
            ('d', "Drums"),
        ),
        max_length=1
    )
    band = models.ForeignKey("Band")`

## URLs and views

A clean, elegant URL scheme is an important detail in a high-quality web application. Django encourages beautiful URL design and doesn’t put any cruft in URLs, like .php or .asp.

To design URLs for an application, you create a Python module called a URLconf. Like a table of contents for your app, it contains a simple mapping between URL patterns and your views.
(credit: https://www.djangoproject.com/start/ )

from django.urls import path

from . import views

urlpatterns = [
    path('bands/', views.band_listing, name='band-list'),
    path('bands/<int:band_id>/', views.band_detail, name='band-detail'),
    path('bands/search/', views.band_search, name='band-search'),
]

## Templates

Django’s template language is designed to strike a balance between power and ease.


