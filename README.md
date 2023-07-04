# Chat App

The Chat App is a simple web application built with Flask that allows users to log in, send messages, and view message history.

## Features

- User Registration: Users can log in by providing their name.
- Home Page: After logging in, users can access the home page where they can send and receive messages.
- Message History: Users can view their message history, including the sender's name, message content, and timestamp.
- Logout: Users can log out of the application.

## Technologies Used

- Python: The backend of the application is developed using Python programming language.
- Flask: Flask is used as the web framework for building the application.
- SQLite: The chat messages are stored in a local SQLite database.
- HTML/CSS: The frontend of the application is built using HTML and CSS.
- JavaScript: JavaScript is used for dynamic interactions on the web pages.

## Installation

### Clone the repository:

git clone <repository-url>

### Change to the project directory:

cd chat-app

### Install the dependencies:

pip install -r requirements.txt

### Run the application:

python app.py

The application will be accessible at http://localhost:5000.

## Usage
Open your web browser and navigate to http://localhost:5000.
Register/Login: Enter your name to log in to the application.
Home Page: You will be redirected to the home page where you can send and receive messages.
Message History: Click on the "Message History" link to view your message history.
Logout: Click on the "Logout" link to log out of the application.

## Database
The chat messages are stored in a local SQLite database. The database file messages.db is automatically created when you run the application for the first time.

## Contribution
Contributions are welcome! If you have any suggestions, improvements, or bug fixes, feel free to open an issue or submit a pull request.

## Old Message Server

The Old Message Server is a custom server implementation using standard Python sockets for a chat application. It provides basic functionality for sending and receiving messages between clients.

### Features

- Server-Client Communication: Clients can connect to the server and exchange messages.
- Broadcast Messages: The server broadcasts messages received from one client to all connected clients.

## FLOW DIAGRAM

Here's a flow diagram illustrating the basic flow of the chat application:


+-----------------+            +-----------------+
|    User Login   |            |   Home Page     |
+-----------------+            +-----------------+
        |                             |
        |                             |
        v                             v
+-----------------+            +-----------------+
|    Login Form   |            |   Message Form  |
+-----------------+            +-----------------+
        |                             |
        |                             |
        v                             v
+-----------------+            +-----------------+
|    Process      |            |    Send         |
|    Login        |            |    Message      |
+-----------------+            +-----------------+
        |                             |
        |                             |
        v                             v
+-----------------+            +-----------------+
|    Redirect     |            |   Broadcast     |
|    to Home      |            |   Message to    |
|    Page         |            |   Connected     |
+-----------------+            |   Clients       |
                               +-----------------+
                                        |
                                        |
                                        v
                               +-----------------+
                               |   Receive       |
                               |   Message       |
                               |   from Server   |
                               +-----------------+
The flow diagram outlines the main steps of the chat application:

User Login: The user provides their name and logs in.
Login Form: The login form is displayed for the user to enter their name.
Process Login: The server processes the login request and saves the user's name.
Redirect to Home Page: The server redirects the user to the home page.
Home Page: The home page is displayed with a message form for sending messages.
Message Form: The user enters a message in the form and submits it.
Send Message: The server receives the message and broadcasts it to all connected clients.
Broadcast Message to Connected Clients: The server sends the message to all connected clients.
Receive Message from Server: Each client connected to the server receives the broadcasted message.

Please note that this flow diagram provides a high-level overview of the chat application's flow
