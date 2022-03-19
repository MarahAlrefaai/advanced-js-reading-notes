
Socket.IO is a library that enables low-latency, bidirectional and event-based communication between a client and a server.

Features
Here are the features provided by Socket.IO over plain WebSockets:

HTTP long-polling fallback
The connection will fall back to HTTP long-polling in case the WebSocket connection cannot be established.

This feature was the #1 reason people used Socket.IO when the project was created more than ten years ago (!), as the browser support for WebSockets was still in its infancy.

Even if most browsers now support WebSockets (more than 97%), it is still a great feature as we still receive reports from users that cannot establish a WebSocket connection because they are behind some misconfigured proxy.

Automatic reconnection
Under some particular conditions, the WebSocket connection between the server and the client can be interrupted with both sides being unaware of the broken state of the link.

That's why Socket.IO includes a heartbeat mechanism, which periodically checks the status of the connection.

And when the client eventually gets disconnected, it automatically reconnects with an exponential back-off delay, in order not to overwhelm the server.

Packet buffering
The packets are automatically buffered when the client is disconnected, and will be sent upon reconnection.

