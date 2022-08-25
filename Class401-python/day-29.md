# Reading: Django Custum User
## Django Best Practices: Custum User Model
### AbstractUser vs AbstractBaseUser
* Both can subclass to extend existing functionality
* AbstractBaseUser requires much more work

### Custom User Model
* update django_project/settings.py
* create new CustomUser model
* create new UserCreation and UserChangeForm
* update the admin

`AUTH_USER_MODEL = "accounts.CustumUser"`

* Update accounts/models.py with a new User model
* Create a new file in the app called forms.py
  * Add classes for CustumUserCreationForm and CustumUserChangeForm

* Update admin.py with CustomUserCreation/ChangeForm class
* Run `makemigrations` and `migrate`

## DjangoX
* A Django starter project
### Setup
* Install it using either Pip, Pipenv, or Docker
* Add environmental variables (maybe use environs)
* Add gunicorn as the production web server
* Update the EMAIL_BACKEND and connect with a mail provider
* Make the admin more sercure
* `django-allauth` supports social authentication if you need/want

