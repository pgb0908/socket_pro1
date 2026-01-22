# Select-based TCP Echo Server and Client

This directory contains a TCP echo server and client that use the `select` function for I/O multiplexing. This allows the server to handle multiple clients concurrently without using multiple threads.

## Files

- `multi_serv.c`: The source code for the select-based echo server.
- `multi_cli.c`: The source code for the echo client.
- `serv`: The compiled executable for the server.
- `cli`: The compiled executable for the client.

## How to Compile

You can compile the server and client using a C compiler like gcc:

```bash
gcc -o serv multi_serv.c
gcc -o cli multi_cli.c
```

## How to Run

1.  **Start the server:**

    ```bash
    ./serv <port>
    ```

    For example:

    ```bash
    ./serv 8080
    ```

2.  **Start the client:**

    ```bash
    ./cli <ip_address> <port>
    ```

    For example:

    ```bash
    ./cli 127.0.0.1 8080
    ```

You can connect multiple clients to the server. The server will echo back any message it receives from any client. To quit a client, type `q` or `Q`.
