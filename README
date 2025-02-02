# CConnect : Socket Programming in C

## Overview
This project is a **Group Chat application** implemented using **Socket programming in C**. It allows multiple clients to connect to a server and exchange messages in real time on any system. The server listens for connections and relays messages between clients.
Make sure to install GCC according to the system you are using.

## Features
- **Multiple Clients**: Supports multiple users connecting to the chat server.
- **Broadcast Messaging**: Messages sent by one client are received by all others.
- **TCP Communication**: Uses TCP sockets for reliable data transfer.
- **Multi-threading**: Uses `pthread` to handle multiple clients concurrently.

---

## Project Structure
```
├── SocketClient_main.c       # Client-side application
├── SocketServer_main.c       # Server-side application
├── socketutil.c              # Utility functions for socket creation and management
├── socketutil.h              # Header file for socket utility functions
└── README.md                 # Project doc
```

---

## Installation & Compilation

### Prerequisites
Make sure you have **GCC** installed on your system. If not, install it using:

**For Ubuntu/Linux:**
```sh
sudo apt update && sudo apt install gcc
```
**For macOS (using Homebrew):**
```sh
brew install gcc
```

---

### Compilation
Use the following commands to compile the server and client programs:

#### Compile the Server
```sh
gcc server_main.c socketutil.c -o server -pthread
```

#### Compile the Client
```sh
gcc client_main.c socketutil.c -o client -pthread
```

---

## Running the Application

### Step 1: Start the Server
Run the following command to start the server:
```sh
./server
```
You should see the output confirming that the server has started successfully:
```
socket was bound successfully
```

### Step 2: Start Clients
Open multiple terminal windows and run the client in each one:
```sh
./client
```
Each client will be prompted to enter a name and begin chatting.

### Step 3: Chat!
- Each client can type a message and send it to the server.
- The server will broadcast the message to all connected clients.
- To exit the chat, type `exit` and press Enter.

---

## How It Works
1. **Server**:
   - Creates a TCP socket.
   - Binds it to an IP and port.
   - Listens for incoming connections.
   - Accepts new clients and starts a new thread for each.
   - Broadcasts received messages to all connected clients.

2. **Client**:
   - Connects to the server using a TCP socket.
   - Sends messages to the server.
   - Listens for incoming messages and prints them.

---

## Example Output :

### Server Output
```
socket was bound successfully
Client connected: IP 127.0.0.1
Elon: Hello everyone!
Jeff: Hi Elon!
```

### Client Output
```
please enter your name:
Katherine
type and we will send (type exit)...
Hello everyone!
The response was Kayla: Hi Katherine!
```
---

## Author
Developed by **Prad Nanduri** for Systems Programming at Penn State.

