# Online Bookstore 

This is a web application project for Browse and purchasing books online. The backend is built with Django REST Framework, and the frontend is developed using Angular.

## Key Features

* **Browse Book Catalog:** Users can view the list of available books.
* **View Book Details:** Display detailed information about each book (title, author, price, etc.).
* **User Authentication:** User registration and login functionality using JWT (JSON Web Tokens) via `djangorestframework-simplejwt`.
* **Shopping Cart:** Users can add books to and manage their shopping cart.
* **Order Placement:** Users can place orders for the books in their cart.
* **Order History:** Authenticated users can view their past orders.
* **Django Admin Panel:** Superusers can manage application data (books, users, orders) through the standard Django admin interface.

## Technologies Used

* **Backend:**
    * Python
    * Django
    * Django REST Framework (`rest_framework`)
    * Django Simple JWT (`rest_framework_simplejwt`) - for authentication
    * Django CORS Headers (`corsheaders`) - for Frontend-Backend communication
    * Database (SQLite default)
* **Frontend:**
    * TypeScript
    * Angular
    * HTML
    * CSS
* **General:**
    * Git / GitHub
    * Python Virtual Environment (`venv`)

## Development Team

* **Bagauova Danara:** ID 23B031233
* **Ibadullayev Asylzhan:** ID 23B030359

## Setup and Run

### Prerequisites

* Python 3.x
* Node.js and npm (or yarn)
* Git

### Backend (Django)

1.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL]
    cd [your-project-folder]/[backend-folder-name]
    ```
2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    # Windows
    .\venv\Scripts\activate
    # macOS/Linux
    source venv/bin/activate
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Ensure you have a `requirements.txt` file listing all packages: `django`, `djangorestframework`, `djangorestframework-simplejwt`, `django-cors-headers`, etc.)*
4.  **Apply migrations:**
    ```bash
    python manage.py migrate
    ```
5.  **Create a superuser (for admin access):**
    ```bash
    python manage.py createsuperuser
    ```
6.  **Run the Django development server:**
    ```bash
    python manage.py runserver
    ```
    *The backend will be available at `http://127.0.0.1:8000/`*

### Frontend (Angular)

1.  **Navigate to the frontend directory:**
    ```bash
    cd [your-project-folder]/[frontend-folder-name]
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    ```
    *(Or `yarn install` if you use Yarn)*
3.  **Run the Angular development server:**
    ```bash
    ng serve --open
    ```
    *The frontend will be available at `http://localhost:4200/` and should open automatically in your browser.*

## Usage

* The main application interface is accessed via the frontend (`http://localhost:4200/`).
* The backend API is available at (`http://127.0.0.1:8000/api/` - *replace `/api/` with your actual API prefix*).
* The Django Admin panel is available at (`http://127.0.0.1:8000/admin/`).

