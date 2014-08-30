django-request-provider
=======================

A middle to get the request from anywhere.


It is inspired on the: django-contrib-requestprovider-1.0.1


Usage
-----


Add the following middleware to *setings.py*:

    MIDDLEWARE_CLASSES=( 
        ...
        'request_provider.middleware.RequestProvider',
        ...
        )


And when you require the request, just do:

    from request_provider.signals import get_request 
    http_request = get_request()

Credits
-------

It seems the code was taken from here: https://github.com/malfaux/snakecheese/tree/master/gadjolib/gadjo/requestprovider
So all the credit should go to: malfaux


