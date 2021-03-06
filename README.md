# django_local_library
Local Library website written in Django(Python3)

This web application creates an online catalog for a small local library, where users can browse available books and manage their accounts.

The main features that have currently been implemented are:

* There are models for books, book copies, genre, language and authors.
* Users can view list and detail information for books and authors.
* Admin users can create and manage models. The admin has been optimised (the basic registration is present in admin.py, but commented out).
* Librarians can renew reserved books

The site is deployed on the server Heroku: https://locallibrary-alexshef.herokuapp.com

*SETUP INSTRUCTIONS for Windows*

  Assuming you have Python setup.

  1. If 'pip' not installed:
        https://pip.pypa.io/en/stable/installing/
  2. Creating an isolated Python environment
  
        `pip install virtualenv`
        
        `virtualenv venv`
        
        `venv\Scripts\activate`
  3. Install the libraries
  
        `pip install -r requirements.txt`
  4. Migrations and creating 'staticfiles' catalog
  
        `python manage.py migrate`
        
        `python manage.py collectstatic`
        
*APPLICATION LAUNCH*

   `python manage.py runserver`
   
   http://127.0.0.1:8000/admin/ - Django administration

   http://127.0.0.1:8000/catalog/ - the library catalog
