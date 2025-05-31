
🧠 My Django Site
A modern Django-based web application designed for publishing content, blogs, attached portfolio or creative posts — built using Django 3.1.5, styled for simplicity, and deployed on Railway for easy cloud access.

🚀 Features
📝 Create, edit, and delete posts

🖼️ Support for images using Pillow

🔐 Admin panel for content management

🕸️ Deployed on Railway (free plan friendly)

⚙️ Lightweight and production-ready using Gunicorn

🏗️ Tech Stack
Layer	Tool / Framework
Backend	Django 3.1.5
Frontend	HTML + CSS
Database	SQLite (default)
Deployment	Railway.app
Image Upload	Pillow
Server	Gunicorn

🔧 Installation
Clone the repository

bash
Copy
Edit
git clone https://github.com/ps-1711/MY_SITE.git
cd your-repo
Create a virtual environment

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run database migrations

bash
Copy
Edit
python manage.py migrate
Run the development server

bash
Copy
Edit
python manage.py runserver
☁️ Deployment on Railway
Upload your code to GitHub.

Go to railway.app → Create New Project → Deploy from GitHub.

Set Start Command in settings:

nginx
Copy
Edit
gunicorn your_project_name.wsgi
Replace your_project_name with the name of the folder containing your settings.py.

Railway will auto-detect a Python project and deploy it. No database plugin required since SQLite is used.

🛠️ Environment Variables
You can define optional variables like:

Variable	Purpose
DEBUG	Toggle Django debug mode
SECRET_KEY	Django secret key
ALLOWED_HOSTS	Hosts allowed to serve app

✅ To Do / Improvements
Add user authentication

Enable comments on posts

Add categories/tags

REST API (optional)

📷 Screenshots
You can include screenshots of:

Home page

Admin panel

Post detail view

(Upload images to a /screenshots folder or link from Railway deployment.)

📜 License
MIT License – free to use, modify, and share.

Visit https://priyanshu-singh.up.railway.app/
