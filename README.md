# chat_app

### A multi-client chat application created using socket programming in C.
- Various clients can chat with each other via a single server.
- The application uses TCP/IP.
- The server manages the different clients in parallel using *threads*.

To run the server process:
```
gcc -pthread server.c -o server
./server <port_no>
```

To run the client process:
```
gcc -pthread client.c -o client
./client <ip_address> <port_no>
```
Everytime you connect a client process to the server, the server sends an **id** for the client.

Syntax for sending messages:
```
<id_of_the_client_you_want_to_chat_with>.<your_msg>
```
Finally, terminate the processes using **Ctrl+D**
