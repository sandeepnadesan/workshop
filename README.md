# Asset Vision

**Asset Vision** is a web-based asset management system designed to help enterprises keep track of their IT assets efficiently. This project leverages **Django** as the backend framework and integrates **React** for a modern, dynamic user interface.

## Table of Contents
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Installation](#installation)
- [CSS Styling](#css-styling)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features
- **Dashboard:** Visual representation of assets and their status.
- **Asset Tracking:** Add, update, and manage assets across locations.
- **Predictive AI:** Insights into asset performance and lifecycle for proactive management.
- **User Management:** Role-based access control for admins and employees.

## Technology Stack
- **Backend:** Django, Python
- **Frontend:** React, JavaScript
- **Database:** MongoDB (`mongodb://localhost:27017/asset-vision`)
- **Other Tools:** Docker, Git

## Installation

### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- Node.js
- MongoDB (running locally)
- Git

### Backend Setup (Django)
1. Clone the repository:
    ```bash
    git clone https://github.com/sandeepnadesan/asset-vision.git
    cd asset-vision
    ```

2. Set up a virtual environment and install dependencies:
    ```bash
    python3 -m venv venv
    source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

3. Set up MongoDB:
    Ensure MongoDB is running on `mongodb://localhost:27017/asset-vision`.

4. Run Django migrations:
    ```bash
    python manage.py migrate
    ```

5. Start the Django development server:
    ```bash
    python manage.py runserver
    ```

### Frontend Setup (React)
1. Navigate to the frontend directory:
    ```bash
    cd frontend
    ```

2. Install the frontend dependencies:
    ```bash
    npm install
    ```

3. Start the React development server:
    ```bash
    npm start
    ```

The project should now be accessible at `http://localhost:3000`.

## CSS Styling

The project includes CSS to ensure a clean and professional look for the user interface. You can find the CSS files in the `frontend/src/styles/` folder.

Here’s an example of a basic `style.css` file to get started:

```css
/* Global Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
}

/* Header */
.header {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}

.header h1 {
    margin: 0;
}

/* Navigation */
.navbar {
    display: flex;
    justify-content: flex-end;
    background-color: #444;
    padding: 10px;
}

.navbar a {
    color: white;
    padding: 14px 20px;
    text-decoration: none;
}

.navbar a:hover {
    background-color: #ddd;
    color: black;
}

/* Dashboard */
.dashboard {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

.dashboard-card {
    background-color: white;
    width: 30%;
    margin: 10px 0;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.dashboard-card h3 {
    margin-bottom: 10px;
    color: #333;
}

.dashboard-card p {
    color: #666;
}
