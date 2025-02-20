# Simple Django Login and Registration

An example of Django project with basic user functionality.

## Screenshots

| Log In | Create an account | Authorized page |
| -------|--------------|-----------------|
| <img src="https://github.com/egorsmkv/simple-django-login-and-register/blob/97dce8bfe5a3f03ae593fe4f1caa75b96959a282/screenshots/login.png" width="200"> | <img src="https://github.com/egorsmkv/simple-django-login-and-register/blob/97dce8bfe5a3f03ae593fe4f1caa75b96959a282/screenshots/create_an_account.png" width="200"> | <img src="https://github.com/egorsmkv/simple-django-login-and-register/blob/97dce8bfe5a3f03ae593fe4f1caa75b96959a282/screenshots/authorized_page.png" width="200"> |

| Password reset | Set new password | Password change |
| ---------------|------------------|-----------------|
| <img src="https://github.com/egorsmkv/simple-django-login-and-register/blob/97dce8bfe5a3f03ae593fe4f1caa75b96959a282/screenshots/password_reset.png" width="200"> | <img src="https://github.com/egorsmkv/simple-django-login-and-register/blob/97dce8bfe5a3f03ae593fe4f1caa75b96959a282/screenshots/set_new_password.png" width="200"> | <img src="https://github.com/egorsmkv/simple-django-login-and-register/blob/97dce8bfe5a3f03ae593fe4f1caa75b96959a282/screenshots/password_change.png" width="200"> |

## Functionality

- Log in
    - via username & password
    - via email & password
    - via email or username & password
    - with a remember me checkbox (optional)
- Create an account
- Log out
- Profile activation via email
- Reset password
- Remind a username
- Resend an activation code
- Change password
- Change email
- Change profile
- Multilingual: English, Russian, and Simplified Chinese


## Installing

### Clone the project

```
git clone https://github.com/egorsmkv/simple-django-login-and-register
cd simple-django-login-and-register
```

### Install dependencies & activate virtualenv

```
pip install pipenv

pipenv install
pipenv shell
```

### Configure the settings (connection to the database, connection to an SMTP server, and other options)

1. Edit `source/app/conf/development/settings.py` if you want to develop the project.

2. Edit `source/app/conf/production/settings.py` if you want to run the project in production.

### Apply migrations

```
python source/manage.py migrate
```

### Collect static files (only on a production server)

```
python source/manage.py collectstatic
```

### Running

#### A development server

Just run this command:

```
python source/manage.py runserver
```
