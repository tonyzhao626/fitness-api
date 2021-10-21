# Backend API for Fitness App

This is the backend API for [Fitness App](https://github.com/tonyzhao626/fitness-app).

## Running

```bash
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
$ createdb eprodb
$ flask db init
$ flask db migrate
$ flask db upgrade
$ export FLASK_APP=app.py
```

- JWT
```bash
>>> import os
>>> os.urandom(24)
$ export SECRET_KEY='code generated above'
```

```bash
(venv)$ flask run
```

API will run at http://localhost:5000

## Routes

- /users/all
- /users/:id
- /users/non_hormonal
- /users/triphasic
- /users/monophasic
- /users/progestin
- /users/register

- /auth/login
- /auth/status
- /auth/logout

- /hormones/non_hormonal
- /hormones/triphasic
- /hormones/monophasic
- /hormones/progestin
