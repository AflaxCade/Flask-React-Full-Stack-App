# Flask-React-Full-Stack-App

Flask-React-Full-Stack-App is a full-stack web application that leverages the power of Flask on the backend and React on the frontend to provide a seamless and interactive user experience. This application is designed to manage contacts, allowing users to perform essential CRUD (Create, Read, Update, Delete) operations on their contact list.

## Features

- Contact Management: Easily manage your contacts by viewing, adding, updating, and deleting them through a user-friendly interface.
- Backend with Flask: The backend is powered by Flask, a lightweight and versatile Python web framework, providing a robust and scalable foundation for data management.
- Frontend with React: The frontend is built using React, a modern JavaScript library for building user interfaces. React enables a dynamic and responsive user experience.
- RESTful API: The communication between the frontend and backend is facilitated by a RESTful API, ensuring efficient data exchange and seamless integration between the two layers of the application.

## Technologies Used

- Flask: A Python web framework for building web applications.
- React: A JavaScript library for building user interfaces.
- RESTful API: Enables communication and data exchange between the frontend and backend.
- SQLite: A lightweight and easy-to-use relational database used for storing contact information.

## Prerequisites Installation

### Requirements

- Python 3.x
- node 20.x

## Getting Started

1. Clone the repository:

```bash
git clone https://github.com/AflaxCade/Flask-React-Full-Stack-App.git
```

2. Navigate to the project directory:

```bash
cd backend
```

3. Create a virtual environment:

```bash
python -m venv venv
```

4. Activate the virtual environment:

- For Windows:

```bash
venv\Scripts\activate
```

- For macOS and Linux:

```bash
source venv/bin/activate
```

5. Install the required dependencies:

```bash
pip install -r requirements.txt
```

6. Run the application:

```bash
python main.py
```

The API will be accessible at http://127.0.0.1:5000/.

## API Endpoints

### Get Contacts

- **URL**: `/contacts`
- **Method**: GET
- **Description**: Retrieves all contacts
- **Response**:
  - Status Code: 200 (OK)
  - Body: JSON object containing a list of contacts

