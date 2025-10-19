My.Jim.Da.WebPro — Complete-Pro ZIP

Includes:
- Django project located in myjimmy_site/
- Static export located in static_site/
- Demo SQLite DB: messages_demo.db with 2 example entries
- Local images (static/img/)

How to run Django locally:
1. Install Python 3.10+, pip.
2. Create venv and activate it.
3. pip install -r requirements.txt
4. From the myjimmy_site directory run migrations and start server:
   python manage.py makemigrations
   python manage.py migrate
   python manage.py createsuperuser  # optional to access admin
   export DJANGO_EMAIL_PASSWORD='your-app-password'  # on Windows use set
   python manage.py runserver

Notes on email sending:
- Use your Gmail account (myjimmythefighter01@gmail.com).
- Create an App Password in your Google Account (Security → App passwords) and set it as DJANGO_EMAIL_PASSWORD in the environment before running the server.
- The contact form posts to /submit/ and will save to the Django DB and attempt to send an email to the same address.

Static export:
- A static-only copy of the site is in static_site/ (open index.html in a browser or host on Netlify/Vercel).

Demo DB:
- messages_demo.db contains a `contact_app_message` table with two example rows.
