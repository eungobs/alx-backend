Alx-backend README
This repository contains solutions for the tasks related to internationalization and localization (i18n) in Flask applications. Each task focuses on different aspects of i18n, from basic setup to more advanced features like handling user preferences and time zones.

Setup
To run the Flask applications in this repository, you'll need to have Python and Flask installed on your system. Additionally, some tasks require the installation of the Flask-Babel extension. You can install it via pip:

$ pip3 install flask_babel==2.0.0

Tasks Overview
Task 0: Basic Flask app
Create a basic Flask app with a single route that displays "Welcome to Holberton" as the page title and "Hello world" as the header.
Task 1: Basic Babel setup
Set up Babel Flask extension and configure available languages as English and French.
Task 2: Get locale from request
Create a function to determine the best-matched locale from the request's accept languages.
Task 3: Parametrize templates
Parametrize templates using gettext function and initialize translations for English and French.
Task 4: Force locale with URL parameter
Implement a way to force a particular locale by passing the locale parameter to the app's URLs.
Task 5: Mock logging in
Mock user login system and display welcome message based on user ID.
Task 6: Use user locale
Update the get_locale function to use a user’s preferred locale if supported.
Task 7: Infer appropriate time zone
Define a function to infer appropriate time zone based on user settings or request header.

Contributor: Elizabeth Eunice Ndzukule.
