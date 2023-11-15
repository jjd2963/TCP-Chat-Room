# TCP-Chat-Room

This Java project implements a client-server chat application using socket communication. The project consists of both a Client and Server class, allowing multiple clients to connect to a central server for real-time messaging.

## Client
The client class establishes a socket connection with the server and handles user input. It creates a separate thread (InputHandler) for continuous input, enabling users to send messages to the server. The client gracefully shuts down upon the "/quit" command, closing connections and releasing resources.

## Server
The server class manages multiple client connections concurrently using a thread pool (ExecutorService). Each client connection is handled by a ConnectionHandler thread, which listens for incoming messages, processes commands (e.g., "/nick" for nickname change), and broadcasts messages to all connected clients. The server gracefully shuts down, closing connections and terminating threads, upon command or exception.

## Features
Bi-Directional Messaging: Clients can send messages to the server, and the server broadcasts them to all connected clients.
Nicknaming: Clients can choose a nickname upon connecting or change it using the "/nick" command.
Graceful Shutdown: Both the client and server implement a clean shutdown mechanism.

## Usage
Compile the Client and Server classes.
Run the server: java Server
Run multiple clients: java Client

## Commands
/nick <new-nickname>: Change your nickname.
/quit: Exit the chat and disconnect from the server.

## Dependencies
Java SE Development Kit (JDK)

## Getting Started
Clone the repository: git clone <repository-url>
Compile the classes: javac Client.java Server.java
Run the server: java Server
Run multiple clients: java Client
Feel free to explore, enhance, and customize this project for your own needs. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

Happy chatting!
