# Basic TCP Echo Server and Client

This directory contains a simple TCP echo server and client. The server listens for incoming connections and echoes back any message it receives from a client.

## Files

- `server_main2.c`: The source code for the echo server.
- `client_main2.c`: The source code for the echo client.
- `serv`: The compiled executable for the server.
- `cli`: The compiled executable for the client.

## How to Compile

You can compile the server and client using a C compiler like gcc:

```bash
gcc -o serv server_main2.c
gcc -o cli client_main2.c
```

## How to Run

1.  **Start the server:**

    ```bash
    ./serv <ip_address> <port>
    ```

    For example:

    ```bash
    ./serv 127.0.0.1 8080
    ```

2.  **Start the client:**

    ```bash
    ./cli <ip_address> <port>
    ```

    For example:

    ```bash
    ./cli 127.0.0.1 8080
    ```

After connecting, you can type a message in the client, and the server will echo it back.
