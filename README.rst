=============================
Tryton-Django
=============================

.. image:: https://badge.fury.io/py/tryton-django.svg
    :target: https://badge.fury.io/py/tryton-django

.. image:: https://travis-ci.org/TinKurbtoff/tryton-django.svg?branch=master
    :target: https://travis-ci.org/TinKurbtoff/tryton-django

.. image:: https://codecov.io/gh/TinKurbtoff/tryton-django/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/TinKurbtoff/tryton-django

Connects Tryton models and database to a Django web application.

Documentation
-------------

The full documentation is at https://tryton-django.readthedocs.io.

Quickstart
----------

Install Tryton-Django::

    pip install tryton-django

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'tryton_django.apps.TrytonDjangoConfig',
        ...
    )

Add Tryton-Django's URL patterns:

.. code-block:: python

    from tryton_django import urls as tryton_django_urls


    urlpatterns = [
        ...
        url(r'^', include(tryton_django_urls)),
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
