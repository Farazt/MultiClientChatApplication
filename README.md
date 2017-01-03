# MultiClientChatApplication
MultiThreadedChatServer that broadcasts as well as sends message to other connected clients using TCP/IP.
Server would read its port from server.config file.
Client would read its port from client.config file.
Server would listen on the port and when the connection establishs with client it would send the client a unique id.
A dedicated thread would handle each client connection.
As multiple threads are using the same resource i use locking to avoid race condition.
Client API:
This API would take selection parameters from the application Layer and act accordingly.
Application Layer runs a dedicated reading thread in order to get data instantly.
Application Layer:
This layer would take message input and show the user options to select from 
Options Include:
Broadcasting the message
Or Specific client interaction 

Server NameSpace:
This NameSpace handles the clients and send and receive messages using tcp/ip according to clients needs.


