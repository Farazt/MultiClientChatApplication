# MultiClientChatApplication
MultiThreadedChatServer that broadcasts as well as sends message to other connected clients using TCP/IP
Server would read its port from server.config file
Client would read its port from client.config file.
Server would listen on the port and when the connection establishs with client it would send the client a unique id.
A dedicated thread would handle each client connection.
As multiple threads are using the same resource i would suggest to use locking to avoid race condition.
Client API:
This API would take selection parameters from the application Layer and act accordingly.
Application Layer runs a dedicated reading thread in order to get data instantly.

