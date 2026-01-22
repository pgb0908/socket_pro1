# Multi-threaded Chat Server and Client

This directory contains a multi-threaded chat server and client. The server can handle multiple clients concurrently, and messages sent by one client are broadcast to all other connected clients.

## Files

- `multi_server.c`: The source code for the multi-threaded chat server.
- `mutli_cli.c`: The source code for the chat client.
- `server`: The compiled executable for the server.
- `cli`: The compiled executable for the client.


## How to Compile

You can compile the server and client using a C compiler like gcc. You need to link the pthread library for the multi-threading functionality.

```bash
gcc -o server multi_server.c -lpthread
gcc -o cli mutli_cli.c -lpthread
```

## How to Run

1.  **Start the server:**

    ```bash
    ./server <port>
    ```

    For example:

    ```bash
    ./server 8080
    ```

2.  **Start the client:**

    ```bash
    ./cli <ip_address> <port> <name>
    ```

    For example:

    ```bash
    ./cli 127.0.0.1 8080 Jules
    ```

You can open multiple client terminals and connect to the server. Messages sent from one client will be visible to all other clients. To quit a client, type `q` or `Q`.
