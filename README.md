# ECommerceWebApp

A full-stack e-commerce web application built with Django. Customers can browse products by category, search the catalog, add items to a cart, place orders, and track them. Products and orders are managed through the Django admin panel.

> Based on the CodeWithHarry Django tutorial project, with the blog and Paytm payment modules removed and the checkout flow simplified.

## Features

- Product catalog grouped by category, with product detail pages
- Search across products
- Shopping cart built with JavaScript (stored in the browser's localStorage)
- Checkout that saves orders to the database
- Order tracker: look up an order by order ID and email to see status updates
- Contact form
- Django admin panel to manage products, orders, order updates, and contact messages

## Tech Stack

- **Backend:** Python, Django
- **Database:** SQLite (Django ORM)
- **Frontend:** HTML, CSS, Bootstrap, JavaScript, jQuery

## Getting Started

1. Clone the repository
   ```
   git clone https://github.com/mhashir12/ECommerceWebApp.git
   cd ECommerceWebApp
   ```
2. Install dependencies
   ```
   pip install django pillow
   ```
3. Apply migrations
   ```
   python manage.py migrate
   ```
4. (Optional) Create an admin user
   ```
   python manage.py createsuperuser
   ```
5. Run the server
   ```
   python manage.py runserver
   ```
6. Open http://127.0.0.1:8000/shop/ in your browser. The admin panel is at http://127.0.0.1:8000/admin/.

## Project Structure

```
mac/     Project settings and root URLs
shop/    Main app: models, views, templates for the store
media/   Product images
```

## Notes

- This is a learning project. Before any real deployment, change `SECRET_KEY`, set `DEBUG = False`, and configure `ALLOWED_HOSTS`.
- Online payment is not implemented; orders are recorded at checkout.

## Author

Mohammad Hashir
