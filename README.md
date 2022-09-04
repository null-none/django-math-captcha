django-math-captcha
=================

Simple match captacha


Installation
------------

    pip install django-math-captacha

Add app in your ``settings.py``

    INSTALLED_APPS = [
        "math_captcha",
    ]


Example

    from django import forms 
    from math_captcha.fields import MathCaptchaField
    
    class MyForm(forms.Form):
        name = models.CharField(max_length=50) 
        captcha = MathCaptchaField()