Smart Register Flask App
This is a simple inventory management and financial tracking application built with Flask, HTML, Tailwind CSS, and JavaScript. It allows users to add new items to inventory, view existing inventory, and modify stock quantities due to sales or damage, while also tracking profit and loss.

Features
Add New Items: Easily add items with unique IDs, names, quantities, and cost prices.

Inventory & Valuation View: See a comprehensive list of all inventory items, including total unique items, total quantity, and total inventory value.

Search Functionality: Quickly find items in the inventory using a search bar.

Stock Modification: Adjust item quantities for sales or damage, with automatic calculation of profit or loss.

Financial Summary: View a real-time summary of total profit and total loss.

Local Storage Persistence: All inventory and financial data are saved locally in the browser, persisting across sessions.

Responsive Design: The application is designed to be usable on various screen sizes (mobile, tablet, desktop).

Project Structure
The project follows a standard Flask application structure:

.
├── app.py
├── requirements.txt
├── Procfile
├── templates/
│   └── index.html
└── static/
    ├── styles.css
    └── script.js

app.py: The main Flask application file, handling routes and rendering templates.

requirements.txt: Lists Python dependencies for the project.

Procfile: Specifies the command to run the application on platforms like Render.

templates/: Contains HTML template files (e.g., index.html).

static/: Contains static assets like CSS (styles.css) and JavaScript (script.js).

Technologies Used
Flask: Python web framework.

HTML5: Structure of the web pages.

Tailwind CSS: Utility-first CSS framework for styling.

JavaScript: Client-side logic for interactive features and data persistence (using Local Storage).

Gunicorn: WSGI HTTP Server for production deployment.

Setup and Installation
Follow these steps to get the Smart Register app up and running on your local machine.

Prerequisites
Python 3.x installed on your system.

Steps
Clone the repository:

git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
cd YOUR_REPOSITORY_NAME

Create a virtual environment (recommended):

python -m venv venv

Activate the virtual environment:

On macOS/Linux:

source venv/bin/activate

On Windows:

venv\Scripts\activate

Install the dependencies:

pip install -r requirements.txt

Run the Flask application:

python app.py

The application will typically run on http://127.0.0.1:5000/. Open this URL in your web browser.

Deployment on Render
This application is configured for easy deployment on Render.com.

Push your code to a GitHub repository.

Create a new Web Service on Render.

Connect your GitHub repository.

Configure the build and start commands:

Build Command: pip install -r requirements.txt

Start Command: gunicorn app:app

Deploy! Render will automatically detect your Procfile and requirements.txt to build and run your application.

Usage
Navigate between "Add Item", "Inventory & Valuation", and "Stock Modification" screens using the navigation buttons.

On the "Add Item" screen, fill in the details and click "Add Item" to add new inventory.

On the "Inventory & Valuation" screen, you can view your current stock and search for items.

On the "Stock Modification" screen, select an item, enter the quantity to change, choose the reason (Sale or Damage), and apply the change. If it's a sale, specify the sale price.
