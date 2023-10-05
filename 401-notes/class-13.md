# Class 13 Notes

## Reading

### Socket.io Chat Example

Explain to a non-technical recruiter what the Chat Example (above) does.

- This is a web application that allows users to chat with each other in real-time. It's similar to how you might send instant messages in a messaging app, but it works within a web browser. Users can open the application in their browsers, join a chat room, and send text messages to others who are also in the same chat room. The unique thing about this chat is that messages appear instantly for everyone in the chat room as soon as they are sent, creating a real-time conversation experience.

What proof of life are we getting on the backend from the above app?

- The "proof of life" on the backend refers to the server's ability to receive, process, and relay messages between connected clients (browsers). When a user sends a message, the server receives that message and then broadcasts it to all other users in the same chat room. This demonstrates that the backend server is active and functioning correctly in handling real-time communication.

Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?

- When using socket.broadcast.emit(), it allows you to send a message to all connected clients except the client associated with the current socket.

### Rooms

What is a room and how might a room be useful?

- It is a virtual channel or group that allows to organize and manage WebSocket connections. They are useful for group communication, privacy, and organization.

How do you join a room?

- You can use the join method:

socket.join('roomName');

how do you leave a room?

- You can use the leave method:

socket.leave('roomName');

### Namespaces

What is a Namespace and what does it allow you to do?

- It is a way to separate WebSocket connections into different communication channels within the same WebSocket server. It allows you to isolate communication, segment functionality and manage permissions.

Each namespace potentially has its own what? (hint: 3 things)

- Set of events, rooms and middleware

Discuss a possible use case for separate namespaces

- A multi-tenant application having separate namespaces are better for organization-specific chat, custom functionality and access control.
