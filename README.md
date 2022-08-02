# wsWonder
> [wsWonder is a Open Source page for make easy Web Scraping
](https://github.com/Zurybr/wsWonder) made by  "[Zurybr](https://zurybr.github.io/main/)"

## Table of Contents:
- [Description](#description)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Using docker](#with-docker)
- [Normal](#without-docker)
- [Usage](#run-it-locally)


## Description
this app is made with Django, django-rest-framework, React.Js and it uses JWT for Authentication. 

### Features
Features included:
- Data modeling with pydantic.
- Data validation.
- CRUD of users.
- CRUD of Tweets.
- SQLAlchemy (MYSQL)
- Docker dev environment
- JWT Authentication
- FastAPI Router
- MyPY

## Requirements:
- Python >= 3.9
- Docker and Docker Compose (Optionally)

## Installation
1. Clone or download de repository:
    ```
    $ git clone https://github.com/Zurybr/wsWonder.git
    ```

2. Open the console inside the project directory and create a virtual environment (You can skip this step if you have docker installed).
    ```bash
    $ python3 -m venv venv
    $ source venv/bin/activate
    ```
    for windows 
    ```cmd
    $ py -m venv venv
    $ .\venv\Scripts\activate
    ```

3. Install the app (You can skip this step if you have docker installed)
    ```bash
    (venv) $ pip install -r requirements.txt
    ```

## Run it locally
Copy the `env.example` file into the same directory with the name `.env`


### With docker
1. Run it with Docker Compose.
```bash
docker-compose up
```

### Without docker
1. Configure the environment variables into the `.env`.
```bash
# App
SECRET_KEY=rVsvupYHUbAgOGNMw0ytII_7tkn_iWkBhktVR_i3Tg8=  # You can leave this dev key as is.
DEBUG=True  # If DEBUG = True, the reload option of uvicorn will be enabled
PORT=8000  # Server port

# Database
DATABASE_URL=mysql+pymysql://${YOUR_USER}:${YOUR_PASSWORD}@${HOST}:${PORT}/${DATABASE NAME}  # Configure your database credentials here.

```

2. Run the server.
```bash
$ python3 manage.py runserver
```

## Basic Usage
Once you are running the server open the [The Browsable API](http://localhost:8000/) and go to the path to checkout the API documentation.
