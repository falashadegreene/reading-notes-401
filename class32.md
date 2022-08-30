# Permissions & Postgresql

## Permissions

Permission basically checks a request and based off the  authentication information given it decides to grant access or denies access. it checks for information from the `request.user` and `request.auth` and determines permissions. Permissions are determined by several factors and if any permissions fail it will raise an exception `exceptions.PermissionDenied` or  `exceptions.NotAuthenticated`. The permission checks fail according to the following: 

- The request was authenticated, but permission was denied. — It will show a HTTP 403 Forbidden response

- The request was not authenticated, a HTTP 403 Forbidden response will be returned.

- The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers. — An HTTP 401 Unauthorized response, with an appropriate WWW-Authenticate header will be returned.

## object level permissions

Object level permissions are used to decide if a user should be allowed to act on a particular object. 

- `exceptions.PermissionDenied` exception is raised if user is not allowed to act on the given object.


## Things I want to know more about

Looking forward to implementing persmissions in real time. 

