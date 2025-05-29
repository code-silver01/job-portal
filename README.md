# 💼 All in one App:

A full-featured collaboration app built with Django and HTML/CSS layouts that allows users to view, post, and manage job listings. The project is in active development and is being expanded to include event and community features to support broader professional networking and collaboration.

---

## 🚀 Features

### ✅ Job Listings (Completed)
- Users can view job postings in a clean card layout.
- Logged-in users can create, edit, and manage job postings through a personal dashboard.
- Supports job filtering and sorting.

---

## 📅 Upcoming Features (In Development)

### 🎉 Events Page
- *Event Feed*: Users can browse through hosted events displayed in a responsive card layout (similar to job listings).
- *Event Creation & Management* (Coming Soon): Users will be able to organize and manage events using the *Dashboard* in the navigation bar.

### 💬 Forums Page
- *Community Chatrooms*: Users can explore various chatroom communities, listed in a card layout format.
- *Private & Group Chatrooms* (Coming Soon): Users will be able to create personal or private chat groups, accessible and manageable via the *Dashboard*.

---

## 🧭 Navigation Overview

- *Home* – Job feed and listings  
- *Dashboard* – Central hub for managing job posts (and soon events & forums)
- *Events* – Browse and create upcoming events (coming soon)
- *Forums* – Community-based discussion/chatrooms (coming soon)

Local environment :

Install
Create a virtual environment

virtualenv venv

Or

python3.11 -m venv venv

Activate it

source venv/bin/activate

Clone the repository and install the packages in the virtual env:

pip install -r requirements.txt

Add .env file.

cp .env.dev.sample .env

Add Github client ID and client secret in the .env file

Run
With the venv activate it, execute:

python manage.py collectstatic

Note : Collect static is not necessary when debug is True (in dev mode)

Create initial database:

python manage.py migrate

Load demo data (optional):

python manage.py loaddata fixtures/app_name_initial_data.json --app app.model_name

Run server:

python manage.py runserver

Default django admin credentials:

email: admin@admin.com password: admin

Run test:
python manage.py test

To dump data:
python manage.py dumpdata --format=json --indent 4 app_name > app_name/fixtures/app_name_initial_data.json
