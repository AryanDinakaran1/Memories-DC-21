# 📝 Memo-Ries

A Django-based web application for personal note-taking and memory management. Users can create, organize, and share notes with ratings, categories, and privacy settings.

## ✨ Features

- **🔐 User Authentication**: Register and login to manage personal notes
- **📝 Note Creation**: Create notes with titles, content, status, ratings, and categories
- **📂 Categorization**: Organize notes into Personal and Professional categories
- **🔒 Privacy Control**: Set notes as Private or Public (Memster)
- **🌐 Social Features**:
  - View public notes from other users
  - User profiles and public note collections
- **⚙️ Note Management**: View, edit, and delete notes
- **📱 Responsive Design**: Mobile-friendly interface with modern UI

## 🛠️ Tech Stack

- **🔧 Backend**: Django 3.2.7
- **🗄️ Database**: SQLite (development), configurable for production
- **🎨 Frontend**: HTML, CSS, JavaScript
- **🎯 Icons**: Font Awesome
- **📊 Analytics**: Google Analytics integration
- **🚀 Deployment**: PythonAnywhere

## 📦 Installation

### 📋 Prerequisites

- 🐍 Python 3.8+
- 🔧 Django 3.2.7
- 📥 Git

### 🏃‍♂️ Local Setup

1. **📥 Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/memories-dc-21.git
   cd memories-dc-21
   ```

2. **🐍 Create a virtual environment**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **📦 Install dependencies**:

   ```bash
   pip install django==3.2.7
   ```

4. **🗄️ Apply database migrations**:

   ```bash
   python manage.py migrate
   ```

5. **👑 Create a superuser (optional, for admin access)**:

   ```bash
   python manage.py createsuperuser
   ```

6. **🚀 Run the development server**:

   ```bash
   python manage.py runserver
   ```

7. **🌐 Access the application**:
   Open your browser and go to `http://127.0.0.1:8000/`

## 📖 Usage

### 🔐 User Registration and Login

1. 🏠 Visit the homepage
2. 📝 Click on "Register" to create a new account
3. 🔑 Or "Login" if you already have an account

### 📝 Creating Notes

1. 🔓 After logging in, click "New Note" from the sidebar
2. 📝 Fill in the note details:
   - 📌 Title
   - 📄 Content
   - 📊 Status
   - ⭐ Rating (1-5)
   - 🏷️ Type (Personal/Professional)
   - 👁️ Visibility (Private/Public)

### ⚙️ Managing Notes

- **👀 View Notes**: Notes are displayed on the home page, categorized by type
- **✏️ Edit Notes**: Click on any note to view details, then use the edit option
- **🗑️ Delete Notes**: Use the delete option from the note view
- **🌍 Public Notes**: View public notes from other users in the "Memster" section

### 👤 User Profiles

- 👥 Visit user profiles to see their public information and shared notes
- 🔗 Access via the "Friends" section or direct links

## 📁 Project Structure

```
memories-dc-21/
├── app/                          # 🏗️ Main Django app
│   ├── migrations/               # 🗄️ Database migrations
│   ├── static/app/               # 🎨 Static files (CSS, JS, images)
│   ├── templates/app/            # 📄 HTML templates
│   ├── admin.py                  # 👑 Admin configuration
│   ├── apps.py                   # ⚙️ App configuration
│   ├── forms.py                  # 📋 Django forms
│   ├── models.py                 # 🏗️ Database models
│   ├── tests.py                  # 🧪 Unit tests
│   ├── urls.py                   # 🛣️ URL patterns
│   └── views.py                  # 👁️ View functions
├── theDiary/                     # ⚙️ Django project settings
│   ├── settings.py               # 🔧 Project settings
│   ├── urls.py                   # 🛣️ Main URL configuration
│   ├── wsgi.py                   # 🌐 WSGI configuration
│   └── asgi.py                   # ⚡ ASGI configuration
├── db.sqlite3                    # 🗄️ SQLite database
├── manage.py                     # 🎮 Django management script
└── README.md                     # 📖 This file
```

## 🏗️ Models

### 📋 Task Model

- `user`: 👤 Username of the note creator
- `title`: 📝 Note title (max 50 characters)
- `contents`: 📄 Note content (max 100,000 characters)
- `status`: 📊 Current status of the note
- `rating`: ⭐ Rating from 1-5
- `noteType`: 🏷️ "Personal" or "Professional"
- `memster`: 👁️ "Private" or "Public" visibility
- `theDate`: 📅 Creation timestamp

## 🚀 Deployment

The application is currently deployed on PythonAnywhere at `https://memories.pythonanywhere.com/`

### ⚙️ Production Settings

- `DEBUG = False`
- `ALLOWED_HOSTS = ["memories.pythonanywhere.com"]`
- 🗄️ Database can be configured for PostgreSQL or other production databases

## 🤝 Contributing

1. 🍴 Fork the repository
2. 🌿 Create a feature branch: `git checkout -b feature-name`
3. 💻 Make your changes and commit: `git commit -am 'Add feature'`
4. ⬆️ Push to the branch: `git push origin feature-name`
5. 📤 Submit a pull request

## 📄 License

This project is open source. Please check the license file for details.

## 📞 Contact

For questions or support, please contact the development team.

---

**📝 Note**: This application includes Google Analytics tracking and AdSense integration for monetization purposes.
