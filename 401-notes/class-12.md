# Class 12 Notes

## Reading

### Web Sockets

What is a Web Socket?

- A WebSocket is a communication protocol that provides full-duplex, bidirectional communication channels over a single TCP connection. In simpler terms, it's a technology that enables real-time, interactive communication between a web server and a client (usually a web browser) without the need for repeated HTTP requests.
Describe the Web Socket request/response handshake and what happens once the connection is established.

Web Sockets provide a standardized way for the server to send content to a client without first receiving a message from that client.

### Socket.io Tutorial

What does the event handler io.on() do?

- Typically used in Node.js applications that implement WebSocket functionality using the Socket.io library. It is used to listen for and handle incoming WebSocket events from clients.

Describe some possible proof of life or proof that the code works as expected

- Using console logs anf server logs help show if the code is working.

What does socket.emit() do?

- Its a function provided by the Socket.io library that allows a server to send WebSocket events to a specific client.

### Socket.io vs Web Sockets

What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

- Difference between Websocket and Socket.io is that Websocket is a communication protocol that enables full-duplex bidirectional communicationover a single TCP connection, where Socket.io is a java library that provided higher level of API.

When would you use Socket.IO?

- Youll use it you need compatibility with wide range of clients. When you need to broadcast messages to multiple clients or building an app with node.js.

When would you use WebSockets?

- You would use it to prioritize low-latency and efficient real-time communication.
