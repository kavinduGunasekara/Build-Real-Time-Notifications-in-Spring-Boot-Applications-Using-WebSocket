# Real-Time Notification System

This repository contains a real-time notification system that provides instant updates across multiple clients without the need for page refreshes.

## Features

- **Real-time updates**: Clients receive updates instantly without requiring a page refresh.
- **Admin panel**: Admin users can broadcast messages to all connected clients.
- **Client views**: End-users automatically receive and display messages in real-time.
- **WebSocket fallback**: Built-in compatibility using SockJS for environments where WebSockets are not supported.

## Technologies Used

- **Backend**: Spring Boot, WebSocket, SockJS
- **Frontend**: HTML, JavaScript

## How It Works

1. **Admin**:
   - Sends updates through a dedicated admin interface.
   - Updates are broadcast to connected clients.

2. **Clients**:
   - Automatically receive and display real-time updates.

3. **Broker**:
   - Uses the `/topic/notifications` channel for message communication between the admin and clients.

## Installation and Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repository-name.git
   cd your-repository-name
   ```

2. **Backend setup:**
   - Ensure you have Java and Maven installed.
   - Navigate to the backend folder and run:
     ```bash
     mvn clean install
     mvn spring-boot:run
     ```

3. **Frontend setup:**
   - Open the `index.html` file in a browser to access the client interface.
   - Use the provided admin interface to broadcast messages.

## Usage

- **Admin Interface:**
  - Use the admin panel to send messages.
  - Messages will be sent to the `/topic/notifications` broker.

- **Client View:**
  - Clients connected to the system will receive and display messages instantly.



---

Feel free to star this repository if you find it helpful!
