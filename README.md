College Suggestion System
This project is a Flask-based web application designed to assist students in finding suitable college suggestions based on their scores and preferences.

Table of Contents
Features
Requirements
Setup
Usage
Project Structure
Routes
Database
Credits
Features
User Registration and Login
Input fields for CET and JEE scores
Gender and Category selection
Location input (manual entry or auto-detection)
Engineering branch selection
College suggestions based on input data
College rankings display (NIRF Rank, NAAC Grade)
Requirements
Python 3.x
Flask
SQLite
Requests
Flask-Session
Werkzeug
Setup
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/college-suggestion-system.git
cd college-suggestion-system
Create a virtual environment:

Copy code
python -m venv venv
Activate the virtual environment:

On Windows:

Copy code
venv\Scripts\activate
On macOS/Linux:

bash
Copy code
source venv/bin/activate
Install the required packages:

Copy code
pip install -r requirements.txt
Set up the database:

Ensure SQLite is installed on your system.

Run the following command to initialize the database:

Copy code
python setup_db.py
Configure Flask environment:

arduino
Copy code
export FLASK_APP=app.py
export FLASK_ENV=development
On Windows, use set instead of export.

Usage
Run the Flask application:

arduino
Copy code
flask run
Open your web browser and navigate to:

arduino
Copy code
http://127.0.0.1:5000
Register a new user or log in with an existing account.

Fill out the form on the details page to receive college suggestions.

Routes
/: Home page
/register: User registration page
/login: User login page
/details: Page for entering scores and preferences
/suggestions: Page displaying college suggestions
/faqs: Frequently Asked Questions page
Database
The project uses an SQLite database named database.db.
The main tables include:
users: Stores user information (id, name, email, password).
colleges: Stores college details.
rankings: Stores college rankings (NIRF Rank, NAAC Grade).
Credits
Developed by Amol Shinde & Rishabhraj Sharma.
Thanks to contributors and the open-source community for libraries and tools used in this project.
Contact
For issues or contributions, please open an issue or a pull request on the GitHub repository.
