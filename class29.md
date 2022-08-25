# Django Custom User Model

Custom User Model has a relationship with the existing user model. It is best to use `AbstractUser` To create a customer user model see below steps. After you complete initial first steps go to settings.py and add app and use the `AUTH_USER_MODEL` config to let Django know use the new custom user model instead of built-in user model.

- update `django_project/settings.py`
- create a new `CustomUser` model
- create new `UserCreation` and `UserChangeForm`
- update the admin
- In `INSTALLED_APPS` add the app at the bottom, then add `AUTH_USER_MODEL` config and the very end of file.

## DjangoX

Djangox is considered to be a starter framework for Django projects that comes with a custom user model out of the box. It extends with social authentication for example like gmail and facebook.

## Things I want to know more about

Is DjangoX just an advanced configuration framework than Django?

