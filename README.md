# Django Parking Management System

This repository contains a Django-based Parking Management System. The application is designed to simplify and automate tasks such as parking spot reservations, payment processing, and administrative functions. It provides an intuitive web interface for users and administrators, along with robust backend functionality.

---

## Features

- **Parking Spot Management**: Manage parking spots for cars and bikes.
- **Payment Processing**: Calculate and process parking charges.
- **Admin Panel**: Dedicated administrative portal to manage parking data.
- **Templates**: Includes reusable HTML templates for a consistent UI.
- **Database Integration**: SQLite database for storing user and parking data.

---

## Project Structure

```
├── parking/                    # Django project directory
│   ├── manage.py               # Django management script
│   ├── db.sqlite3              # SQLite database
│   ├── templates/              # HTML templates
│   │   ├── basic/              # Reusable base templates
│   │   │   ├── charges_basic.html
│   │   │   ├── base.html
│   │   │   └── adinput.html
│   │   ├── charges_bike.html   # Bike charges page
│   │   ├── charges_car.html    # Car charges page
│   │   ├── admin.html          # Admin panel
│   │   ├── parkInfobike.html   # Bike parking info
│   │   ├── parkInfocar.html    # Car parking info
│   │   ├── index.html          # Landing page
│   │   ├── pay.html            # Payment page
│   │   ├── data_in.html        # Data input page
│   │   ├── final.html          # Final confirmation page
│   │   ├── start.html          # Start page
│   │   ├── dateby.html         # Date-based filtering page
│   │   ├── data.html           # Parking data page
│   │   ├── option.html         # Options page
│   │   └── out.html            # Checkout page
│   ├── parking/                # Django app directory
│   │   ├── settings.py         # Django project settings
│   │   ├── __init__.py         # Python package initializer
│   │   ├── urls.py             # URL routing
│   │   ├── asgi.py             # ASGI configuration
│   │   ├── admin.py            # Django admin configuration
│   │   ├── views.py            # View logic
│   │   └── wsgi.py             # WSGI configuration
└── static/                     # Static assets
    └── images/
        ├── ICON/               # Icon files
        │   ├── site.webmanifest
        │   └── about.txt
        └── ICON.zip            # Compressed icon assets
```

---

## Installation

### Prerequisites

- Python 3.8+
- Django 3.2+

### Steps to Run Locally

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/django_parking_management_system.git
   cd django_parking_management_system/parking
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Start the Development Server**:
   ```bash
   python manage.py runserver
   ```

6. **Access the Application**:
   Open a browser and navigate to `http://127.0.0.1:8000/`.

---

## Technologies Used

- **Framework**: Django
- **Database**: SQLite
- **Frontend**: HTML, CSS

---

## Future Enhancements

- Integrate a payment gateway for real-time payments.
- Add support for additional parking lot types.
- Implement responsive design for mobile compatibility.
