# Epoll TCP Echo Server and Client

This directory contains a TCP echo server and client that use the `epoll` API for efficient I/O. This allows the server to handle a large number of concurrent connections with low overhead.

## Files

- `epoll_server.c`: The source code for the epoll-based echo server.
- `epoll_client.c`: The source code for the epoll-based echo client.
- `epoll_echo 서버 모델.PNG`: A diagram illustrating the server model.

## How to Compile

You can compile the server and client using a C compiler like gcc:

```bash
gcc -o epoll_server epoll_server.c
gcc -o epoll_client epoll_client.c
```

## How to Run

1.  **Start the server:**

    ```bash
    ./epoll_server
    ```

    The server will listen on port 12000.

2.  **Start the client:**

    ```bash
    ./epoll_client
    ```

After connecting, you can type a message in the client, and the server will echo it back. You can also run multiple clients simultaneously to see how the server handles them. To quit the client, type `q` or `Q`.
