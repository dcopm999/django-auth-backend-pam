=====
Usage
=====

To use Django authorization backend with pam in a project, add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'auth_backend_pam.apps.AuthBackendPamConfig',
        ...
    )

Add Django authorization backend with pam's URL patterns:

.. code-block:: python

    from auth_backend_pam import urls as auth_backend_pam_urls


    urlpatterns = [
        ...
        url(r'^', include(auth_backend_pam_urls)),
        ...
    ]
