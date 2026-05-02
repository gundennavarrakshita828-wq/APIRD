Markdown# 🍹 APIRD: Drinks Management API

A robust RESTful API built with **Django 5.1** and **Django REST Framework** for managing a catalog of drinks. This project is structured for global scalability with extensive localization support.

---

## 📁 Project Structure
```text
APIRD/
├── APIRD/              # Project Configuration
│   ├── settings.py     # Global Settings
│   ├── urls.py         # Root URL Routing
│   ├── asgi.py         # ASGI configuration for deployment
│   └── wsgi.py         # WSGI configuration for deployment
├── Drinks/             # Main Application Logic
│   ├── migrations/     # Database Evolution files
│   ├── templates/      # HTML templates (e.g., index.html)
│   ├── models.py       # Database Schema
│   ├── serializers.py  # Data Serialization logic
│   ├── views.py        # API Request/Response Handling
│   └── admin.py        # Admin interface registration
├── venv/               # Virtual Environment & Django i18n Files
├── manage.py           # Django Admin Utility
└── db.sqlite3          # Local SQLite Database
🚀 Getting Started1. Environment SetupThe project is configured for Python 3.13. To activate the environment:  Windows: venv\Scripts\activate  Unix/macOS: source venv/bin/activate  2. Database InitializationApply the migrations stored in Drinks/migrations/ to set up your db.sqlite3 file:  Bashpython manage.py migrate
3. Running the Development ServerLaunch the project locally:Bashpython manage.py runserver
The API will be available at http://127.0.0.1:8000/.  🛠️ Core ComponentsData Model (models.py)Defines the attributes and structure of a "Drink" entry in the database.  API Serializer (serializers.py)Utilizes Django REST Framework to convert model instances into JSON format for client consumption.  Global Localization (venv/locale/)The project includes pre-compiled .mo and source .po files for over 50 languages, including[cite: 1]:Arabic (ar)[cite: 1]German (de)[cite: 1]Spanish (es)[cite: 1]French (fr)[cite: 1]Japanese (ja)[cite: 1]Russian (ru)[cite: 1]📡 API EndpointsMethodEndpointDescriptionGET/drinks/List all drinks in the database[cite: 1]POST/drinks/Add a new drink to the collection[cite: 1]GET/drinks/<id>/Retrieve details for a specific drink[cite: 1]PUT/drinks/<id>/Update an existing drink record[cite: 1]DELETE/drinks/<id>/Remove a drink from the database[cite: 1]🔧 Technologies UsedFramework: Django 5.1[cite: 1]API Toolkit: Django REST Framework[cite: 1]Database: SQLite 3[cite: 1]Environment: Virtualenv (Python 3.13)[cite: 1]Version Control: Git[cite: 1]Generated for the APIRD Project - 2026
