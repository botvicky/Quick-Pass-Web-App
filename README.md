# QuickPass Web App

QuickPass is a web application built with Flask that provides user authentication and management functionality. It allows users to register, log in, and manage their profiles, with additional features for admin users.

## Features

- User registration and login system
- User profile management
- Role-based access control (User and Admin roles)
- Admin dashboard for user management
- Secure password hashing
- Session management with "Remember me" functionality
- Responsive design for various screen sizes

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7 or higher installed
- pip (Python package manager) installed
- Git installed (for cloning the repository)

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/botvicky/Quick-Pass-Web-App.git
   cd Quick-Pass-Web-App
   ```

2. Create a virtual environment:
   ```
   python -m venv venv
   ```

3. Activate the virtual environment:
   - On Windows:
     ```
     venv\Scripts\activate
     ```
   - On macOS and Linux:
     ```
     source venv/bin/activate
     ```

4. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Configuration

1. Open `app.py` and replace the secret key with a secure, random string:
   ```python
   app.config['SECRET_KEY'] = 'your_secure_secret_key_here'
   ```

2. If you want to use a different database, update the `SQLALCHEMY_DATABASE_URI` in `app.py`:
   ```python
   app.config['SQLALCHEMY_DATABASE_URI'] = 'your_database_uri_here'
   ```

## Usage

1. Run the application:
   ```
   python app.py
   ```

2. Open a web browser and navigate to `http://localhost:5000`

3. Register a new user account

4. Log in with your credentials

5. Explore the features:
   - Update your profile information
   - If you're an admin, access the admin dashboard

## Creating an Admin User

To create an admin user:

1. Register a new user through the application
2. Access the SQLite database file (`users.db`) using a SQLite browser (e.g., DB Browser for SQLite)
3. Open the `user` table
4. Find the user you want to make an admin and change their `role` column value to 'admin'
5. Save the changes to the database

## Contributing

Contributions to QuickPass are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch: `git checkout -b feature-name`
3. Make your changes and commit them: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

Please ensure your code adheres to the project's coding standards and include tests for new features.

## Contact

For any questions, feedback, or support, please contact Victoria Mahuni at mahunivictor13@gmail.com.
