# TCP-Chat-Room

This Java project introduces a simple socket-based chat application with a client-server architecture. The project utilizes the java.net package to establish a socket connection, allowing communication between a client and a server.

Features
Socket Communication: The client establishes a socket connection with a server running on the local machine (127.0.0.1) and port 9999.
Bi-Directional Messaging: The client sends messages to the server, and the server echoes them back to the client, creating a basic chat interaction.
Input Handling: The application employs a separate thread for handling user input, allowing for real-time communication. The user can input messages, and the application will send them to the server.
Usage
Compile the Client class.
Run the compiled class to start the client.
The client connects to the server, and you can start typing messages in the console.
Type "/quit" to gracefully exit the application.
How It Works
The client establishes a socket connection with the server.
Input handling is managed by a separate thread (InputHandler), enabling continuous message input.
User messages are sent to the server, and the server echoes them back to the client.
The application provides a clean shutdown mechanism with the "/quit" command.
Dependencies
Java SE Development Kit (JDK)
Getting Started
Clone the repository: git clone <repository-url>
Compile the Client class: javac Client.java
Run the client: java Client
Feel free to explore, enhance, and customize this project for your own needs. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.
