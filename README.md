# Realtime Chat Application

This is a realtime chatroom application using Django and WebSockets.

## Setup

#### - Create Virtual Environment

###### # Mac

```
python3 -m venv venv
source venv/bin/activate
```

###### # Windows

```
python3 -m venv venv
(Powershell:) .\venv\Scripts\Activate.ps1
```

```
(or Command Prompt:) venv\Scripts\activate
(or Git Bash:) source venv/Scripts/activate
```

<br>

#### - Install dependencies

```
pip install --upgrade pip
pip install -r requirements.txt
```

<br>

#### - Migrate to database

```
python manage.py migrate
python manage.py createsuperuser
```

<br>

#### - Run application

```
python manage.py runserver
```

<br>

#### - Generate Secret Key ( ! Important for deployment ! )

```
python manage.py shell
from django.core.management.utils import get_random_secret_key
print(get_random_secret_key())
exit()
```
