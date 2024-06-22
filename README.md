# flask-file-upload-app
This is a simple web application built with Flask for uploading and displaying files. It supports images, PDFs, and text files and shows a preview for images.

## Features
File Upload: Users can upload images, PDFs, and text files.
File Preview: Uploaded images are displayed with a preview.
File Listing: All uploaded files are listed with links to view or download them.
## Project Structure
arduino
Copy code

flask-file-upload-app/
│
├── app/                         # Main application folder
│   ├── static/                  # Static files (e.g., CSS, JavaScript)
│   │   └── uploads/             # Folder to store uploaded files
│   ├── templates/               # HTML templates
│   │   └── index.html           # Main template for file upload and display
│   ├── __init__.py              # Initializes the Flask application
│   └── routes.py                # Defines routes for file uploading and viewing
│
├── requirements.txt             # Python dependencies
├── Procfile                     # Specifies commands for deploying to Heroku
└── runtime.txt                  # Specifies the Python version for Heroku

app/static/: Contains static files and uploaded files.
app/templates/: Contains HTML templates.
app/__init__.py: Initializes the Flask app.
app/routes.py: Contains the routes for handling file uploads and displaying files.
requirements.txt: Lists the dependencies.
Procfile: Specifies commands for deployment on Heroku.
runtime.txt: Specifies the Python runtime version for deployment.
## Prerequisites
Python 3.10 or above
pip for managing Python packages
## Installation
### Clone the repository:

bash
Copy code
git clone https://github.com/<username>/flask-file-upload-app.git
cd flask-file-upload-app
### Create a virtual environment:

bash
Copy code
python3 -m venv venv
### Activate the virtual environment:

Windows:

bash
Copy code
venv\Scripts\activate
macOS/Linux:

bash
Copy code
source venv/bin/activate
### Install the dependencies:

bash
Copy code
pip install -r requirements.txt
## Configuration
Upload Folder: Files are uploaded to app/static/uploads/.
Allowed File Types: Images (png, jpg, jpeg, gif), PDFs (pdf), and text files (txt).
File Size Limit: Maximum file size is set to 16 MB.
## Running the App
Set the Flask environment variables:

bash
Copy code
export FLASK_APP=app
export FLASK_ENV=development
For Windows (Command Prompt):

bash
Copy code
set FLASK_APP=app
set FLASK_ENV=development
Run the Flask app:

bash
Copy code
flask run
Access the app:
Open a browser and go to http://127.0.0.1:5000.

## Deployment
Deploying to Heroku
Create a Heroku account: Heroku

Install the Heroku CLI: Heroku CLI

Login to Heroku:

bash
Copy code
heroku login
Create a Heroku app:

bash
Copy code
heroku create your-app-name
Deploy the app:

bash
Copy code
git push heroku master
Open the app:

bash
Copy code
heroku open
### Deploying to Render
Create a Render account: Render

Create a new Web Service:

Choose your GitHub repository.
Follow the prompts to deploy.
![Screenshot (329)](https://github.com/nilupultharanga/flask-file-upload-app/assets/88283925/04653d1e-6493-493a-ba54-7b7766b273d6)



## Contributing
Fork the repository.
Create a new branch.
Make your changes.
Submit a pull request.
## License
This project is licensed under the MIT License. See the LICENSE file for details.
