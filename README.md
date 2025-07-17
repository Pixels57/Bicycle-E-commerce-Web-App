# Bicycle E-Commerce Web Application

A full-featured Django web application for buying and selling bicycles online. This platform allows users to create accounts, list their bicycles for sale, browse available listings, and manage their inventory.

## 🚲 Features

- **User Authentication**: Registration, login, and logout functionality
- **Bicycle Listings**: Create, view, edit, and delete bicycle listings
- **Image Upload**: Upload and display bicycle images
- **Search & Filter**: Browse and filter listings by various criteria
- **User Dashboard**: Manage personal listings
- **Responsive Design**: Bootstrap-powered responsive UI
- **Admin Panel**: Django admin interface for site management

## 🏗️ Deployment History

**Note**: This application was previously deployed and hosted on cloud infrastructure but has been migrated to local development due to high resource costs:

- **Previous Setup**: 
  - Hosted on Heroku (Production server)
  - AWS RDS PostgreSQL (Database)
  - AWS S3 (File storage)

- **Current Setup**: Local development environment to avoid ongoing expenses

## 🚀 Quick Start

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Bicycle-E-commerce-Web-App
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv .venv
   
   # On Windows
   .venv\Scripts\activate
   
   # On macOS/Linux
   source .venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run database migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser (optional)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Start the development server**
   ```bash
   python manage.py runserver
   ```

7. **Access the application**
   - Open your browser and go to: `http://127.0.0.1:8000/`
   - Admin panel: `http://127.0.0.1:8000/admin/`

## 📱 How to Use

### For Buyers

1. **Browse Listings**
   - Visit the homepage to see featured listings
   - Click "All Listings" to browse all available bicycles
   - Use filters to find specific types of bikes

2. **View Details**
   - Click on any listing to see detailed information
   - View high-quality images and specifications

### For Sellers

1. **Create Account**
   - Click "Register" to create a new account
   - Fill in your details and verify your email

2. **Login**
   - Use your credentials to log into your account

3. **Create Listings**
   - Click "New Listing" to add a bicycle for sale
   - Fill in details: brand, model, price, condition, etc.
   - Upload clear photos of your bicycle
   - Add detailed description

4. **Manage Listings**
   - Visit "My Listings" to see all your posted bicycles
   - Edit or delete listings as needed
   - Update prices and availability

### For Administrators

1. **Access Admin Panel**
   - Go to `/admin/` and login with superuser credentials
   - Manage users, listings, and site content
   - Monitor site activity and moderate content

## 🛠️ Technology Stack

- **Backend**: Django 5.2.1 (Python web framework)
- **Database**: SQLite (local development)
- **Frontend**: HTML, CSS, JavaScript, Bootstrap 5
- **Forms**: Django Crispy Forms with Bootstrap 5
- **Filtering**: Django Filter
- **File Storage**: Local file system
- **Authentication**: Django built-in auth system


## 🔧 Configuration

### Environment Settings

The application is configured for local development with:
- `DEBUG = True`
- SQLite database
- Local file storage
- Development server settings

### For Production Deployment

If you want to deploy this application again, you'll need to:

1. **Update settings.py**:
   - Set `DEBUG = False`
   - Configure `ALLOWED_HOSTS`
   - Set up environment variables for sensitive data

2. **Database**:
   - Configure PostgreSQL or another production database
   - Update database settings in `DATABASES`

3. **File Storage**:
   - Set up AWS S3 or another cloud storage service
   - Configure `DEFAULT_FILE_STORAGE` and related settings

4. **Security**:
   - Use environment variables for secret keys
   - Configure HTTPS
   - Set up proper CORS settings
