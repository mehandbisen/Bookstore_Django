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
### Screenshots
![Screenshot 2025-04-25 164332](https://github.com/user-attachments/assets/66e4560c-cbfc-493d-ab97-ac983436b089)
![Screenshot 2025-04-25 164257](https://github.com/user-attachments/assets/722140ef-1ed6-48ed-8f3e-5517c98efc36)
![Screenshot 2025-04-25 164206](https://github.com/user-attachments/assets/54979b3b-1919-4167-89b8-2f8cee39299f)


## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/bookstore.git
cd bookstore
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` doesn't exist, create one:
>
> ```bash
> pip freeze > requirements.txt
> ```

### 3. Configure MySQL Database

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

### 4. Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create a Superuser

```bash
python manage.py createsuperuser
```

### 6. Start the Development Server

```bash
python manage.py runserver
```
