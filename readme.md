# Project Title: mfdw_site

## Description
A web application built using Django 3, inspired by "Build a Website with Django 3" by Nigel George. This project demonstrates how to create user-specific views, manage data interaction, and implement robust authentication.

## Features
- **User Authentication**: Includes registration, login, and logout functionalities.
- **Custom Templates**: Tailored templates for a better user experience.
- **Data Management**: Efficient interaction between models, views, and templates.
- **Access Control**: Restricted access to data, ensuring unauthorized users cannot view sensitive information.
- **Dynamic Page Creation**: A custom `Page` model allows the creation of dynamic pages for the site.
- **Quote Request Management**: A custom `Quote` model enables users to submit quote requests.

## Page Model
The `Page` model includes the following fields:
- **Title**: A string field for the page title.
- **Permalink**: A slug field for generating user-friendly URLs.
- **Last Update Date**: A DateTime field to track when the page was last updated.
- **Content**: A text field for the main content of the page.

This model enables the creation of multiple pages within the site, each with its own unique content and URL.

## Quote Model
The `Quote` model includes the following fields:
- **Name**: The name of the user requesting the quote.
- **Position**: The user's job title or position.
- **Company**: The name of the user's company.
- **Address**: The user's company address.
- **Phone**: The user's contact number.
- **Email**: The user's email address.
- **Web**: The user's company website.
- **Description**: A description of the quote request.
- **Site Status**: The current status of the site (e.g., active, inactive).
- **Priority**: The priority level of the quote request.
- **Job File**: An optional field for uploading relevant documents.
- **Submitted Date**: The date the quote request was submitted.
- **Quote Date**: The date the quote was provided.
- **Quote Price**: The estimated price for the requested quote.
- **Username**: The username of the user submitting the quote request.


This model allows users to easily request quotes and provides a structured way to manage these requests.

## Technologies Used
- **Django 3**
- **Python 3**
- **SQLite/PostgreSQL** 

## Installation
Follow these steps to set up the project locally:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ahmadfaraz2/nigel-django3.git
   ```
2. **Navigate to the project directory**:
    ```bash 
    cd mfdw_root
    ```
3. **Create a virtual environment**:
    ```bash 
    cd python -m virtualenv venv
    ```
4. **Activate the virtual environment**:
    - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```
5. **Install the requirements**:
    ```bash
    python -m pip install -r requirements.txt
    ```

## Usage
To run the project, use the following command:
```bash
    python manage.py runserver
```

# Screenshots
![Homepage](Screenshots/Screenshot%20(13).png)
*Homepage, about us and services pages are created through `page` model*

![Contact Us](Screenshots/Screenshot%20(551).png)
*Contact Us Page*

![User Registration](Screenshots/Screenshot%20(558).png)
*User Registration Page*

![User Registration Success page](Screenshots/Screenshot%20(561).png)
*User Registration Success Page*

![Login Page](Screenshots/Screenshot%20(560).png)
*Login Page*

![Quote Request Page](Screenshots/Screenshot%20(555).png)
*A form to quote request*

![All Quotes](Screenshots/Screenshot%20(556).png)
*Show all quotes submitted by the login user*

![Quote Detail](Screenshots/Screenshot%20(557).png)
*A Detail Quote View*