# Joseph Garkida · Portfolio

A personal portfolio website built with Django, with an admin panel for managing every part of the site. No HTML editing is needed to update content.

**Live site:** [https://your-domain.com]

![Home page](screenshots/home-dark.png)

## Features

- **Editable content:** name, about text, skills, experience, education, services, and social links, all managed from the Django admin
- **Projects:** project cards, each with its own page, extra screenshots, and technology filters
- **Blog:** Markdown posts with drafts, tags, reading time, and RSS feeds
- **Contact form:** saves every message to the database, emails me, and has spam protection (hidden field and rate limiting)
- **Testimonials** and a downloadable **CV**
- **Dark and light mode**, remembered in the visitor's browser
- **Responsive design** with a mobile side menu
- **Simple page-view counter** and support for Plausible, Umami, or Cloudflare analytics
- **Automated tests** for pages, the contact form, the blog, and the admin

## Tech stack

Python, Django, HTML, CSS, JavaScript, SQLite (PostgreSQL in production), WhiteNoise, Gunicorn, Font Awesome

## Run it locally

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
python -m venv venv
source venv/Scripts/activate        # Windows (Git Bash)
pip install -r requirements.txt
cp .env.example .env                # then set SECRET_KEY in .env
python manage.py migrate
python manage.py seed_content       # optional starter content
python manage.py createsuperuser
python manage.py runserver
```

Site: http://127.0.0.1:8000/ · Admin: http://127.0.0.1:8000/admin/

## Tests

```bash
python manage.py test
```

## Project structure

```
config/      settings and main URLs
core/        home page, projects, contact form, site settings
blog/        posts, blog pages, RSS feeds
templates/   HTML templates
static/      CSS, JavaScript, images
```

## Deployment

Se
