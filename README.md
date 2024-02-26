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

### Create Contact

- **URL**: `/create_contact`
- **Method**: POST
- **Description**: Creates a new contact
- **Request Body**: JSON object with the following properties:
  - `firstName` (string): First name of the contact (required)
  - `lastName` (string): Last name of the contact (required)
  - `email` (string): Email address of the contact (required)
- **Response**:
  - Status Code: 201 (Created)
  - Body: JSON object with a success message
 
Here is Json example for creating new contact

```json
{
    "firstName": "John",
    "lastName": "Doe",
    "email": "john.doe@example.com"
}
```

### Update Contact

- **URL**: `/update_contact/<int:user_id>`
- **Method**: PATCH
- **Description**: Updates an existing contact
- **URL Parameters**:
  - `user_id` (integer): ID of the contact to be updated
- **Request Body**: JSON object with the following optional properties:
  - `firstName` (string): Updated first name of the contact
  - `lastName` (string): Updated last name of the contact
  - `email` (string): Updated email address of the contact
- **Response**:
  - Status Code: 200 (OK)
  - Body: JSON object with a success message

### Delete Contact

- **URL**: `/delete_contact/<int:user_id>`
- **Method**: DELETE
- **Description**: Deletes a contact
- **URL Parameters**:
  - `user_id` (integer): ID of the contact to be deleted
- **Response**:
  - Status Code: 200 (OK)
  - Body: JSON object with a success message

## For the React Frontend

1. Navigate to the project directory in different terminal:

```bash
cd frontend
```

2. Install the dependencies:

```bash
npm install
```

3. Running the Application:

```bash
npm run dev
```

The React app will be accessible at http://localhost:5173.

make sure you are runing both backend and the frontend server at the same time.

### Snapshot of the app

![App Screenshot](https://github.com/AflaxCade/Flask-React-Full-Stack-App/blob/main/Snapshot.png?raw=true)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
