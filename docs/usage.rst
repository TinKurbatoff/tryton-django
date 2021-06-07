=====
Usage
=====

To use Tryton-Django in a project, add it to your `INSTALLED_APPS`:

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
