- ## Code 401 - *Class 12 readings (web sockets) *

#### What is a Web Socket?


A WebSocket is a communication protocol that allows for real-time, two-way communication between a client and a server over a single TCP connection. It enables persistent connections and eliminates the need for multiple HTTP requests, facilitating efficient and low-latency data exchange for real-time web applications.


#### Describe the Web Socket request/response handshake and what happens once the connection is established.



The WebSocket handshake begins with the client sending an HTTP request to upgrade to the WebSocket protocol. The server responds with an HTTP response, acknowledging the upgrade. Once the handshake is complete, the connection is upgraded to WebSocket, enabling real-time bidirectional communication between the client and server.


#### Web Sockets provide a standardized way for the server to send content to a client without first receiving a *request* from that client.


#### What does the event handler io.on() do?

The `io.on()` event handler is used in server-side JavaScript frameworks like Socket.IO to listen for specific events emitted by connected clients. When an event is received, the associated callback function is executed, allowing the server to respond or perform actions based on the event.

#### Describe some possible proof of life or proof that the code works as expected

Unit Testing: Write and execute unit tests to verify individual components or functions within the code. These tests validate the expected behavior of specific code units and help identify any issues or discrepancies.

Integration Testing: Conduct integration tests to assess the interaction and compatibility between different modules or components of the code. These tests focus on ensuring that the integrated system functions correctly as a whole.

Test Cases and Test Suites: Create a comprehensive set of test cases and test suites that cover different scenarios and edge cases. This allows you to systematically verify the code's behavior across various inputs and conditions.


#### What does socket.emit() do?

`socket.emit()` is a function used in WebSocket or Socket.IO frameworks to send events from the client to the server or from the server to connected clients. It facilitates event-based communication by sending specific events and associated data between the client and server.


#### What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

WebSocket is a low-level communication protocol, while Socket.IO is a JavaScript library that provides a higher-level API and additional features for real-time communication.

#### When would you use Socket.IO?

Socket.IO is used when you need real-time, bidirectional communication in applications such as chat, collaboration, real-time analytics, multiplayer games, notifications, IoT, and social media integration. It provides a simple and reliable API with fallback mechanisms for broader browser compatibility.

#### When would you use WebSockets?


WebSockets are used for real-time, bidirectional communication in applications such as chat, collaboration, dashboards, multiplayer games, notifications, live feeds, and remote control. They provide low latency and efficient communication for real-time updates and interactions.



