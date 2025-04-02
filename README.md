# Django Project: Calculator and Book Management System

This project is a Django-based web application developed as part of a college practical. It consists of two main applications:
1. **Calculator App**: A simple calculator for performing basic arithmetic operations.
2. **Book Management System**: A CRUD-based system for managing books, including adding, viewing, editing, and deleting book records.

---

## Features

### Calculator App
- Perform basic arithmetic operations: addition, subtraction, multiplication, and division.
- User-friendly interface with modern styling.

### Book Management System
- **Create**: Add new books with details like title, author, publication date, ISBN, and genre.
- **Read**: View a list of all books or details of a specific book.
- **Update**: Edit the details of an existing book.
- **Delete**: Remove a book from the system.
- Modern, responsive UI using Bootstrap.

---

## Installation

Follow these steps to set up the project on your local machine:

### Prerequisites
- Python 3.10 or higher
- Django 5.1.7
- A virtual environment (recommended)

### Steps
1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd Django
   ```

2. **Set Up a Virtual Environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Linux/Mac
   venv\Scripts\activate     # On Windows
   ```

3. **Install Dependencies**
   ```bash
   pip install django
   ```

4. **Apply Migrations**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Run the Development Server**
   ```bash
   python manage.py runserver
   ```

6. **Access the Application**
   Open your browser and navigate to:
   - **Home Page**: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
   - **Calculator App**: [http://127.0.0.1:8000/calc/](http://127.0.0.1:8000/calc/)
   - **Book Management System**: [http://127.0.0.1:8000/books/](http://127.0.0.1:8000/books/)

---

## Project Structure

```
Django/
├── calculator/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
├── calc/
│   ├── templates/
│   │   └── calc/
│   │       └── calculator.html
│   ├── views.py
│   ├── urls.py
├── books/
│   ├── templates/
│   │   └── books/
│   │       ├── create_book.html
│   │       ├── book_list.html
│   │       ├── book_detail.html
│   │       ├── update_book.html
│   │       └── delete_book.html
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── forms.py
├── templates/
│   └── index.html
├── db.sqlite3
└── manage.py
```

---

## Overview of the Applications

### 1. **Calculator App**
- **URL**: `/calc/`
- **Description**: A simple calculator that allows users to perform basic arithmetic operations. The result is displayed dynamically on the page.

### 2. **Book Management System**
- **URL**: `/books/`
- **Description**: A CRUD-based system for managing books. Users can:
  - Add new books.
  - View a list of all books.
  - View details of a specific book.
  - Edit book details.
  - Delete books.

---

## Technologies Used
- **Backend**: Django 5.1.7
- **Frontend**: HTML, CSS, Bootstrap 5.3
- **Database**: SQLite (default Django database)


## License
This project is for educational purposes only and is not intended for production use.

---

## Author
**Faraaz**  
Developed as part of a college practical.