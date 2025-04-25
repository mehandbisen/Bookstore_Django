# 📚 Django Bookstore Web App

A fully functional and responsive bookstore web application built with Django. It allows users to register, login, and view a list of books. Admin users can also add new books. The app uses Bootstrap for styling and supports MySQL as the backend database.

---

## 🚀 Features

- 🔐 User Registration & Authentication (Login/Logout)
- 👤 Admin-Only Book Addition
- 📖 Public Book Listing
- 🎨 Responsive UI with Bootstrap 5
- ✅ CSRF-protected Forms
- 🗃️ MySQL Database Integration

---

## 🛠 Tech Stack

- **Backend**: Django 5.2 (Python 3.12)
- **Frontend**: HTML5, Bootstrap 5
- **Database**: MySQL
- **Language**: Python

---

## 📁 Project Structure

```
bookstore/
├── books/
│   ├── migrations/
│   ├── templates/
│   │   └── books/
│   │       ├── base.html
│   │       ├── book_form.html
│   │       ├── book_list.html
│   │       ├── home.html
│   │       ├── login.html
│   │       ├── logout.html
│   │       └── register.html
│   ├── admin.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
├── bookstore/
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── manage.py
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/bookstore.git
cd bookstore
```

### 2. Create and Activate Virtual Environment

```bash
python -m venv env
# Windows
env\Scripts\activate
# Linux/Mac
source env/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` doesn't exist, create one:
>
> ```bash
> pip freeze > requirements.txt
> ```

### 4. Configure MySQL Database

In `bookstore/settings.py`:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'bookstore_db',
        'USER': 'root',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### 5. Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Create a Superuser

```bash
python manage.py createsuperuser
```

### 7. Start the Development Server

```bash
python manage.py runserver
```

Open your browser and go to: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

## 🔐 Admin Panel

Visit [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/) and log in with your superuser credentials to manage books and users.

---

## 📝 Future Improvements

- 📸 Add book cover uploads
- 🔍 Implement search and filtering
- 🛒 Add shopping cart and checkout
- 🌐 Add REST API support for books

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 💬 Feedback & Contributions

Feel free to fork this repo, suggest changes, or submit a pull request!

Made with ❤️ using Django.