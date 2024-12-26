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


## Usage

- **Admin Interface:**
  - Use the admin panel to send messages.
  - Messages will be sent to the `/topic/notifications` broker.

- **Client View:**
  - Clients connected to the system will receive and display messages instantly.


![Screenshot 2024-12-26 230102](https://github.com/user-attachments/assets/5bd81243-1ef3-43a1-966a-c6c4c0b82c22)
![Screenshot 2024-12-26 225936](https://github.com/user-attachments/assets/9b037f3b-3af9-45eb-ad3b-aad89460c8fc)

---

Feel free to star this repository if you find it helpful!
