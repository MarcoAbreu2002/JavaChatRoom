# JavaChatRoom

## Project Overview

**JavaChatRoom** is a simple chat application designed to enable communication between multiple clients through a central server. The server broadcasts messages sent by any client to all other connected clients, ensuring that everyone stays updated in real-time.

### Key Features

- **Centralized Messaging**: All clients communicate via a central server that handles message broadcasting.
- **Concurrent Handling**: The server manages multiple client connections simultaneously, creating separate threads for each client to ensure smooth communication and prevent the main thread from blocking.
- **Data Integrity & Availability**: The server is designed with a focus on reliability, ensuring that it remains available and maintains the integrity of data at all times.

### Server Logging

The server maintains a detailed log of all activities, stored in the `server/server.log` file. This log includes:

- Messages sent and received.
- Client connection and disconnection events.
- Clients waiting for a connection slot.
- Timestamps for each event.

### Configuration

All server settings are stored in the 'server/server.config' file. This configuration file should be modified to adjust any necessary server parameters. If your project requires additional settings, they should be included in this configuration file as well.

### Instalation
To install this simple application, just clone this repository to your local machine.

   ```bash
   git clone https://github.com/MarcoAbreu2002/JavaChatRoom.git
   ```

## Running the Application

### Starting the Server

1. Compile and run the server application.
2. The server will start listening for incoming client connections.

### Connecting Clients

1. After starting the server, you can connect multiple clients by running the `Client.main` method.
2. To open multiple client instances:
   - Go to the client’s file in your IDE.
   - Select "Edit Configurations...".
   - Click "Modify options".
   - Enable "Allow multiple instances".

This setup will allow you to run multiple client tabs and simulate a chatroom environment with several participants.
