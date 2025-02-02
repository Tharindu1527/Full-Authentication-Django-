# Django Full Authentication System with NextJS

A comprehensive authentication system built with Django REST Framework and NextJS, featuring JWT authentication, Google OAuth, and AWS email verification services. This project provides a robust, secure, and scalable authentication solution with a modern frontend interface.

## Features

- **Multiple Authentication Methods**
  - JWT (JSON Web Token) Authentication
  - Google OAuth Integration
  - Email/Password Authentication
  - Password Reset Functionality

- **Email Verification**
  - AWS SES Integration for Email Services
  - Custom Email Templates
  - Verification Link Generation

- **Secure Backend**
  - Django REST Framework
  - Djoser Authentication Views
  - PostgreSQL Database
  - Custom User Model
  - COOkIES 

- **Modern Frontend**
  - NextJS 13+ Framework
  - Responsive Design
  - Protected Routes
  - Authentication State Management

## Tech Stack

### Backend
- Django
- Django REST Framework
- Djoser
- PostgreSQL
- Simple JWT
- AWS SES

### Frontend
- NextJS
- React
- Axios
- TailwindCSS

## Installation

### Backend Setup

1. Clone the repository
```bash
git clone https://github.com/Tharindu1527/Full-Authentication-Django-.git
cd Full-Authentication-Django-
```

2. Create and activate virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Setup PostgreSQL database and update settings

5. Configure environment variables
```bash
# .env
DEVELOPMENT_MODE = "True"
DJANGO_SECRET_KEY = ""
DEBUG = "True"
AWS_SES_ACCESS_KEY_ID = ""
AWS_SES_SECRET_ACCESS_KEY = ""
AWS_SES_REGION_NAME = "us-east-1"
AWS_SES_FROM_EMAIL = ""
DOMAIN = "localhost:3000"
AUTH_COOKIE_SECURE = False
GOOGLE_AUTH_KEY =  
GOOGLE_AUTH_SECRET_KEY = "
DATABASE_NAME=
DATABASE_USER=
DATABASE_PASSWORD=
DATABASE_HOST=
DATABASE_PORT=
```

6. Run migrations
```bash
python manage.py migrate
```

7. Start the development server
```bash
python manage.py runserver
```

### Frontend Setup

1. Navigate to frontend directory
```bash
cd frontend
```

2. Install dependencies
```bash
npm install
```

4. Run the development server
```bash
npm run dev
```

## API Endpoints

## Postman Setup

1. Import the provided Postman collection
2. Set up environment variables:
   - `BASE_URL`: Your API base URL
   - `JWT_TOKEN`: Your authentication token

Collection includes all API endpoints with example requests and responses.

## AWS SES Setup

1. Create AWS account
2. Set up SES service
3. Verify email addresses
4. Create SMTP credentials
5. Update environment variables

## Security Features

- JWT token authentication
- Secure password hashing
- Email verification
- Protected API endpoints
- CORS configuration
