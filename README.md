# E-commerce Full Project Using Django With SSLCOMMERZ Payment System
 This e-commerce project is full solution for any kind of e-commerce business.I used in this project django as framework and sslcommerz as payment. SSLCOMMERZ for bangladesh payment system.If you want i will implement any kind of payment gateway in this project, like Paypal, Stripe, Nochex etc.
 
 ![E-commerce Full Project](https://github.com/NowshadRuhan/E-commerce-Full-Project-Using-Django-With-SSLCOMMERZ-Payment-System/blob/main/home.png?raw=true) 
 
 ## About Project:
**In this project i used  four apps, media folder, static folder, templates and others pip library/packages, And most important sslcommerz for payment system.**

## About Crispy forms in python:
Django-crispy-forms supports several frontend frameworks, such as Twitter Bootstrap (versions 2, 3, and 4), Uni-form and Foundation. You can also easily adapt your custom company's one, creating your own, see the docs for more information. You can easily switch among them using CRISPY_TEMPLATE_PACK setting variable.

### Installing django-crispy-forms:

**Install latest stable version into your python environment using pip:**
- pip install django-crispy-forms

**If you want to install development version (unstable), you can do so doing:**
- pip install git+git://github.com/django-crispy-forms/django-crispy-forms.git@dev#egg=django-crispy-forms


**Once installed add crispy_forms to your INSTALLED_APPS in settings.py:**
```
INSTALLED_APPS = (
    ...
    'crispy_forms',
)
```
**For add template packs within django-crispy-forms:**
```
#bootstrap, bootstrap3, bootstrap4, uni-from
CRISPY_TEMPLATE_PACK = 'bootstrap4'
```

### About Media Files in Django:
In Django, files which are uploaded by the user are called Media or Media Files. Here are some examples:
1. A user uploaded image, pdfs, doc files etc while publishing a post.
2. Images of products in an e-commerce site.
3. User's profile image. etc...

**Just as with static files, to serve media files we have do add some configurations in our settings.py file.**

#### Media Files Configurations:
Media files depend upon two configurations,
1. MEDIA_ROOT,
2. MEDIA_URL

**In settings.py file:**
```
STATICFILES_DIRS = [
    os.path.join(BASE_DIR, 'static'),
]

MEDIA_ROOT  = os.path.join(BASE_DIR, 'media')
MEDIA_URL = '/media/'
```

**In the main project urls.py file:**
```
from django.conf.urls import url, include
from django.contrib import admin
from django.conf import settings
from django.conf.urls.static import static

urlpatterns = [
    url(r'^admin/', admin.site.urls),
] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
```
### About static File in Django:
In static folder we store our all of css, js, bootstrap file to use those file in our project.

**Settings added**
```
from django.conf import settings
```
**static and static_url added**
```
from django.conf.urls.static import static
```

**for load static folder in templates**
```
{% load static %}
```
# About Project Apps:
   **In this project i used four web-app this are App_Login, App_Shop, App_Order & App_Payment. And database i used in this project is sqlite-3.**
   
1. App-Login:
   - In app-login i make a fully custom model for login and registation. Where i create one custom model name is Profile and it is connected with User model by One To One connection. 
   - Also  I used email as a unique field for this project. For unique email i need to customize Django user model.I used BaseUserManager, AbstractBaseUser, PermissionsMixin for customized user model.
   - In app-login i also used two custom forms for profile model and user login model. The forms are Sign-Up-Form and Profile-Form.
   - For Sign-Up-Form I also used Django auth class UserCreationForm.
   - Though, it's a e-commerce project, so that I used email and password for login and registation.And all others profile things need to update after login.
   
    ![E-commerce Full Project](https://github.com/NowshadRuhan/E-commerce-Full-Project-Using-Django-With-SSLCOMMERZ-Payment-System/blob/main/e-commerce-login-auth.png?raw=true) 
   
2. App-Shop:
   - In app-shop I create two custom model. One of Category and other on is Product.
   - Category model used for make product in Category wise. example: Food, Clothing, Music etc..
   
   
   
    
   
   
   
   
