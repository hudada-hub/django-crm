# Django CRM System

A comprehensive CRM (Customer Relationship Management) system built with Django 6.0.3, designed for mechanical industry companies.

## Features

- **Customer Management**: Complete CRUD operations for customers
- **Contact Management**: Track customer contacts and interactions
- **Product Management**: Manage products with details and pricing
- **Opportunity Tracking**: Sales funnel management with stages
- **Order Processing**: Create and manage orders with items
- **Activity Tracking**: Log customer interactions (calls, emails, meetings)
- **Task Management**: Create and assign tasks with due dates
- **File Management**: Upload and manage customer files and contracts

## Technology Stack

- **Backend**: Django 6.0.3, Python 3.13+
- **API**: Django REST Framework
- **Async Tasks**: Celery
- **Cache**: Redis
- **Database**: SQLite (development), PostgreSQL/MySQL (production)
- **Frontend**: Django Templates, Custom CSS
- **Internationalization**: i18n support (Chinese/English)

## Getting Started

### Prerequisites
- Python 3.13+
- pip
- Redis (for caching and Celery)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/hudada-hub/django-crm.git
   cd django-crm
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate  # Windows
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create superuser**
   ```bash
   python manage.py createsuperuser
   ```

6. **Start development server**
   ```bash
   python manage.py runserver
   ```

## Project Structure

```
myproject/
├── myproject/              # Project configuration
├── crm/                    # CRM application
│   ├── models.py          # Data models
│   ├── views.py           # Function-based views
│   ├── views_cbv.py       # Class-based views
│   ├── api.py             # REST API
│   ├── forms.py           # Forms
│   ├── templates/         # HTML templates
│   └── static/            # Static files
├── templates/             # Global templates
└── manage.py             # Management script
```

## API Endpoints

- `/api/customers/` - Customer API
- `/api/contacts/` - Contact API
- `/api/products/` - Product API
- `/api/opportunities/` - Opportunity API
- `/api/orders/` - Order API
- `/api/activities/` - Activity API
- `/api/tasks/` - Task API

## License

MIT
