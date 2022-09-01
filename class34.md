# API Deployment

## Django Settings Best Practices

- `settings_local.py` - That allows you to extend environment-specific settings. Settings is a good foundation for your project if you set it up right and is a very important step in a Django project. Example:

`ALLOWED_HOSTS = ['example.com']`
`DEBUG = False`
`DATABASES = {`
    `'default': {`
        `'ENGINE': 'django.db.backends.postgresql',`
        `'NAME': 'production_db',`
        `'USER': 'user',`
        `'PASSWORD': 'password',`
        `'HOST': 'db.example.com',`
        `'PORT': '5432',`
        `'OPTIONS': {`
            `'sslmode': 'require'`
        }
    }
}

`from .settings_local import *`

A few pros and cons of `settings_local.py`

pros

- Secrets not in VCS.
cons

- You can lose some of your Django environment settings
- settings_local.py can have some non-obvious logic
- settings_local.example (in VCS) must be set to share the default Django configurations for developers.

## SSH

(Secure Shell Protocol) aka SSH, is considered a remote admin protocol that lets users access control, and change their remote servers over the internet. Example of SSH commmand: `ssh {user}@{host}`

## Things I want to know more about 

Interested to see more of `settings_local.py` and how it benefits when building a django project. 

