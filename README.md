# Resturant_Project

A Django-based web application for restaurant management, featuring menu browsing, table booking, customer feedback, cart functionality, and an admin dashboard. The project uses Bootstrap for responsive design and supports image uploads and Google Maps integration.

---

## Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Customization](#customization)
- [License](#license)

---

## Features

- **Home Page:** Slider, featured offers, customer reviews.
- **Menu:** Browse food items by category.
- **Table Booking:** Reserve tables with email confirmation.
- **Feedback:** Submit ratings and images.
- **Cart:** Add menu items to cart (AJAX).
- **About:** Restaurant information and Google Maps location.
- **User Authentication:** Login, signup, logout.
- **Admin Panel:** Manage menu, bookings, feedback, and users.
- **Responsive Design:** Mobile-friendly with Bootstrap.

---

## Project Structure

```
Resturant_Project/
├── Base_App/
│   ├── migrations/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
├── Media/
│   ├── feedback/
│   └── items/
├── Static/
│   ├── css/
│   ├── fonts/
│   ├── images/
│   └── js/
├── Template/
│   ├── about.html
│   ├── base.html
│   ├── book_table.html
│   ├── feedback.html
│   ├── home.html
│   ├── login.html
│   └── menu.html
├── Resturant_Project/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── db.sqlite3
├── manage.py
└── requirements.txt
```

---

## Setup Instructions

### 1. Clone the Repository

```sh
git clone https://github.com/yourusername/feane-restaurant.git
cd feane-restaurant
```

### 2. Create and Activate Virtual Environment

```sh
python -m venv venv
venv\Scripts\activate  # On Windows
```

### 3. Install Dependencies

```sh
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the project root (if needed):

```
GOOGLE_MAPS_API_KEY=your-google-maps-api-key
EMAIL_HOST_USER=your-email@example.com
EMAIL_HOST_PASSWORD=your-email-password
```

Update email and API settings in `Resturant_Project/settings.py` as required.

### 5. Apply Migrations

```sh
python manage.py migrate
```

### 6. Create Superuser (for admin panel)

```sh
python manage.py createsuperuser
```

### 7. Collect Static Files

```sh
python manage.py collectstatic
```

### 8. Run the Development Server

```sh
python manage.py runserver
```

Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.

---

## Usage

- **Home:** View offers and reviews.
- **Menu:** Browse and add items to cart.
- **Book Table:** Reserve a table and get confirmation.
- **Feedback:** Submit ratings and images.
- **About:** View restaurant info and location.
- **Login/Signup:** Access user features.
- **Admin:** Manage menu, bookings, feedback, and users.

---

## Technologies Used

- Django 5.x
- Bootstrap 4
- jQuery, OwlCarousel, Isotope, Nice Select
- SQLite3 (default)
- Google Maps API
- Font Awesome

---

## Customization

- Change images in `Static/images`
- Update menu items and categories via Django admin
- Modify styles in `Static/css/style.css`
- Edit templates in `Template/`

---

## License

This project is licensed under the MIT License.

---

**For issues or contributions, please open an issue or pull request on GitHub.**
