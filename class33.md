# Authentication & Production Server

## JSON Web Token

It is used to tranismit information between parties as a JSON object. It can be digitally signed with secret or private key. (HMAC, RSA or ECDSA.) Web tokens are typically useful for the following:

- Authorization
- information exchange

Web Token Structure looks like the following: `xxxxx.yyyyy.zzzzz`

- Header
- Payload
- Signature

## DRF JWT Authentication

JWT uses a signature issued by the backend and the signature is called upon verified request. Any information changed by the client in the header it will invalidate the signature. To validate the signature it will have to use the application's signature `SECRET_KEY`


## Django Runserver Is Not Your Production Server

In order to run Django in production it is more effienct to use a production ready web server and handled by WSGI application server. the function `uwsgi.py` it creates a Python object that shows the incoming request, then calls a code and creates a response object then passed along to WSGI server.

## Things I want to know more about 

Want to learn more about putting JSON Web token to use. 
