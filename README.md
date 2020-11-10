# E-commerce Full Project Using Django With SSLCOMMERZ Payment System
 This e-commerce project is full solution for any kind of e-commerce business. I used in this project django as framework and sslcommerz as payment. SSLCOMMERZ for bangladesh payment system. If you want i will implement any kind of payment gateway in this project, like Paypal, Stripe, Nochex etc.
 
 ![Quick-Share-Profile](https://github.com/NowshadRuhan/E-commerce-Full-Project-Using-Django-With-SSLCOMMERZ-Payment-System/blob/main/home.png?raw=true) 
 
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
**For add template packs within django-crispy-forms: **

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
