# Django Study Project 🧠💻

This is a result of Django project based on a tutorial by [**@SteinOveHelset**](https://github.com/SteinOveHelset) on his YouTube video at [Code With Stein](https://youtu.be/m3nYd_IFZuU?si=gfT9p9uXlUuEC1an). It serves as a great starting point for learning Django basics including models, views, templates, and routing.

📺 **Credits**  
Huge thanks to [Stein Helset](https://github.com/SteinOveHelset) for the original video tutorial.  
If you're just starting out with Django, check out his video and follow step-by-step instruction — it's super beginner-friendly and clear.

**Note**  
This repository contains additional features that make project result different from original video tutorial.

---

## 🛠 Setup Instructions (for Forked Repository Users)

Follow the steps below after forking this repository to your own GitHub account:


### 1. Clone your forked repo

Clone your repository and navigate to it:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```


### 2. Create a Virtual Environment

Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
```


### 3. Create a `.env` File

Use the `.env.example` file in the repository as a reference.  
To generate a new Django `SECRET_KEY`, run the following in a Python shell:

```python
from django.core.management.utils import get_random_secret_key
print(get_random_secret_key())
```

Then create a `.env` file in the root of your project and add:

```env
SECRET_KEY=your_generated_secret_key_here
DEBUG=True
```


### 4. Install Required Packages

Install dependencies listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```


### 5. (Optional) Make Migrations

Run this only if you've added or modified models:

```bash
python manage.py makemigrations
```


### 6. Apply Migrations to Create the Database

Apply all migrations to set up your local database:

```bash
python manage.py migrate
```


### 7. Run the Development Server

Start your local development server:

```bash
python manage.py runserver
```


### ✅ You're All Set!
Visit http://127.0.0.1:8000/ in your browser to view the project running locally.  
Happy coding! ✨