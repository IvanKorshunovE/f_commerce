# FCommerce

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

- `git clone https://github.com/IvanKorshunovE/f_commerce`
- `python -m venv venv`
- `source venv/bin/activate`
- `pip install -r requirements.txt`
- `go to the root directory and type 'export FLASK_APP=run.py' in the terminal`
- `populate .evn file from .env.sample`
- `open Python console, type 'from market import db'`
- `db.create_all()`
- `flask run`
