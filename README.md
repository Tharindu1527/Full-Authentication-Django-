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
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=postgresql://user:password@localhost:5432/db_name
AWS_ACCESS_KEY_ID=your-aws-access-key
AWS_SECRET_ACCESS_KEY=your-aws-secret-key
AWS_SES_REGION=your-aws-region
GOOGLE_OAUTH_CLIENT_ID=your-google-client-id
GOOGLE_OAUTH_CLIENT_SECRET=your-google-client-secret
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

3. Configure environment variables
```bash
# .env.local
NEXT_PUBLIC_API_URL=http://localhost:8000
NEXT_PUBLIC_GOOGLE_CLIENT_ID=your-google-client-id
```

4. Run the development server
```bash
npm run dev
```

## API Endpoints

### Authentication Endpoints
```
POST /auth/users/ - Register new user
POST /auth/jwt/create/ - Obtain JWT token
POST /auth/jwt/refresh/ - Refresh JWT token
POST /auth/users/reset_password/ - Reset password
POST /auth/users/reset_password_confirm/ - Confirm password reset
GET /auth/users/me/ - Get current user
POST /auth/google/ - Google OAuth authentication
```

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

## Project Structure

```
django-full-auth/
├── backend/
│   ├── accounts/          # Custom user model and authentication
│   ├── core/              # Core functionality
│   └── config/            # Project settings
├── frontend/
│   ├── pages/             # NextJS pages
│   ├── components/        # React components
│   └── services/          # API services
└── docs/                  # Documentation
```

## Security Features

- JWT token authentication
- Secure password hashing
- Email verification
- Protected API endpoints
- CORS configuration
- SSL/TLS support
- Request rate limiting

## Development

### Running Tests
```bash
# Backend tests
python manage.py test

# Frontend tests
npm run test
```

### Code Formatting
```bash
# Backend
black .
flake8

# Frontend
npm run lint
```

## Deployment

1. Set up production environment variables
2. Configure CORS settings
3. Set up SSL certificate
4. Configure database settings
5. Set up static files serving
6. Deploy backend to preferred hosting (e.g., AWS, DigitalOcean)
7. Deploy frontend to Vercel or similar platform

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

[Add your chosen license here]

## Contact

[Your Name] - [your.email@example.com]

Project Link: [https://github.com/[your-username]/django-full-auth](https://github.com/[your-username]/django-full-auth)
