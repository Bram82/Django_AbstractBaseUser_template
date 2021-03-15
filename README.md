####Project goal:
To create a reusable app that extends from AbstractBaseUser and uses email as the identifier.  

###Project description
* The app_accounts is set up so that the user uses email for verification. This is done by extending the  
AbstractBaseUser in the `models.py` file of the app.  
* A new file `managers.py` is created to be able to create users using an email as identifier.
* In `forms.py` custom forms are defined for the django-admin to use when a user is created or altered.
* In 'admin.py' a CustomUserAdmin class is created. This controls the django-admin forms for user creation   
 and altering.
* To use app_accounts in another project:
    * app_accounts should be added to `INSTALLED_APPS` in the settings file
    * `AUTH_USER_MODEL = 'app_accounts.User'` Should also be added to the settings file  
    to set the custom user model as the project standard.
    * run `python manage.py makemigrations` and `python manage.py migrate` to create the models in the database.
  
####Steps to be taken / Possible improvements
 

