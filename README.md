# LittleLemon Restaurant Project

## Overview

LittleLemon Restaurant is a Django-based web application for managing a restaurant's menu and bookings. The project includes features such as displaying the menu, handling bookings, and providing a simple web interface for customers and staff.

## Content

### Project Structure

The project follows a typical Django structure, with the main components being:

- **littlelemon:** The main project directory.
  - **restaurant:** The Django app handles restaurant-related functionality (menu, bookings).
  - **templates:** Contains HTML templates for rendering views.
  - **static:** Holds static files like CSS (styles.css) and images.


### Features

- **Menu Management:**
  - Add, update, and delete menu items.
  - View a list of available menu items with details such as title, price, and inventory.

- **Booking System:**
  - Record customer bookings with details like the customer's name, number of guests, and booking date.
  - Utilizes Django REST framework's powerful `ModelViewSet` for handling booking information.

- **Authentication:**
  - Secure user authentication using Djoser, providing features like token authentication and user registration.


### Usage

1. Clone the repository:

    ```bash
    git clone https://github.com/aymane66/littlelemon.git
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Run migrations:

    ```bash
    python manage.py migrate
    ```

4. Start the development server:

    ```bash
    python manage.py runserver
    ```

5. Access the application at [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

### Dependencies

- Django 4.2.7
- djangorestframework
- djoser

## What I Have Learned

Throughout the development of LittleLemon Restaurant, I have gained valuable experience in:

- Setting up a Django project for a restaurant management system.
- Configuring Django settings, including database and authentication settings.
- Implementing RESTful APIs using Django REST framework.
- Integrating token-based authentication with Djoser.
- Creating models for database interaction and registering them with the Django admin.
- Writing serializers to transform Django models into JSON representations.
- Defining URL patterns and views for handling HTTP requests.
- Utilizing class-based views and view sets for efficient code organization.
- Configuring and using a MySQL database with Django.
- Collaborating with middleware for request/response processing.

## Future Enhancements

- I am currently dedicating my attention to Backend technologies and I will complete the front end for this project in the near future.
- Your feedback is appreciated.



Explore the project freely. Contact me for issues or suggestions.

