=============================
Django authorization backend with pam
=============================

.. image:: https://badge.fury.io/py/django-auth-backend-pam.svg
    :target: https://badge.fury.io/py/django-auth-backend-pam

.. image:: https://travis-ci.org/dcopm999/django-auth-backend-pam.svg?branch=master
    :target: https://travis-ci.org/dcopm999/django-auth-backend-pam

.. image:: https://codecov.io/gh/dcopm999/django-auth-backend-pam/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/dcopm999/django-auth-backend-pam

Django pam auth

Documentation
-------------

The full documentation is at https://django-auth-backend-pam.readthedocs.io.

Quickstart
----------

Install Django authorization backend with pam::

    pip install django-auth-backend-pam

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'auth_backend_pam',
        ...
    )

Add Django authorization backend with pam's URL patterns:

.. code-block:: python

    urlpatterns = [
        ...
        path('auth_backend_pam/', include('auth_backend_pam.urls')),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox


Development commands
---------------------

::

    pip install -r requirements_dev.txt
    invoke -l


Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
