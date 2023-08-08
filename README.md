# Flask Market App

Welcome to the Flask Market App! This project is a web-based application built using the Flask framework, designed for managing a virtual marketplace. Users can register, log in, buy and sell items, and keep track of their budgets. Below is an overview of the project structure, key features, and how to get started.

## Key Features

- **User Registration and Login**<br>
Users can register with a unique username, email address, and password.
Passwords are securely hashed using the bcrypt library.
Existing usernames and email addresses are validated during registration.
- **Budget Management**<br>
Each user has a budget, which is initially set to $5000.
The budget is updated when users purchase or sell items.
- **Item Purchase and Selling**<br>
Users can purchase items from the market if they have sufficient funds.
Users can sell items back to the market to increase their budget.
- **Flask-Login Integration**<br>
The application uses the Flask-Login extension to manage user sessions.
Users can log in and log out of their accounts.
- **HTML Templates and Forms**<br>
HTML templates are used to render different pages with dynamic data.
Forms are implemented using Flask-WTF for user input validation.


## Installing using GitHub (macOS)

- `git clone https://github.com/IvanKorshunovE/my_cinema_application`
- `cd my_cinema_application`
- `python -m venv venv`
- `source venv/bin/activate`
- `pip install -r requirements.txt`
- `set POSTGRES_HOST=<your db hostname>`
- `set POSTGRES_DB=<your db name>`
- `set POSTGRES_USER=<your db user>`
- `set POSTGRES_PASSWORD=<your db password>`
- `set SECRET_KEY=<your secret key>`


After you have done everything before:
- `python manage.py migrate`
- `python manage.py runserver`

How to run this in docker:
- `docker-compose build`
- `docker-compose up`

To create a superuser in Django within a Docker container, you can follow these steps:
- First, identify the name of the container running your Django application. You can use the docker ps command to list all running containers and find the container name associated with your Django app.
- Once you have the container name, you can use the docker exec command to execute commands inside the container. The command should be structured as follows:
- `docker exec -it <container_name> python manage.py createsuperuser`

Endpoints:
- create user via /api/user/register/
- get access token via /api/user/token/

Features
- JWT authenticated 🔒
- Admin panel /admin/
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie sessions
- Managing orders and tickets
- Filtering movies and movie sessions
