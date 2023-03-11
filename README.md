# Flask Chat Application

This is a simple chat application built with Flask and Flask-SocketIO. The application allows users to join a chat room by creating a new one or entering an existing one. Users can send messages to the chat room and view messages from other users in real-time.

## Prerequisites

Before running this application, you will need to have the following installed on your machine:

- Python 3
- Flask
- Flask-SocketIO

## Running the Application

To run the application, execute the following command in your terminal:

>python main.py


The application will then be available at `http://localhost:5000`.

## Features

- User can create a new chat room with a randomly generated code or join an existing one.
- User can send messages to the chat room, which will be displayed in real-time to all users in the room.
- User can view messages that have been sent in the chat room.

## Code Structure

The application is built with Flask and Flask-SocketIO. The main code is contained in `app.py`. The `generatecode` function is used to generate a random code for a new chat room. The `home` function is used to handle requests to the home page, where users can enter their name and select whether to create a new chat room or join an existing one. The `room` function is used to handle requests to the chat room page, where users can view messages and send new messages.

The application uses Flask-SocketIO to handle WebSocket connections for real-time communication between clients. The `connect` and `disconnect` functions are used to handle socket connections and disconnections. The `message` function is used to handle incoming messages from clients, which are then broadcasted to all clients in the room.

## Contributing

If you find a bug or would like to contribute to this application, feel free to submit an issue or pull request on GitHub.
