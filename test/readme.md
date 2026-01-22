# Java Client-Server Test Application

This directory contains a simple client-server application written in Java.

## Files

- `Boot.java`: The main class to start the server and client.
- `Server.java`: This appears to be a compiled Java class file (`Server.class`) that has been misnamed. It contains the server logic.
- `Client.java`: This also appears to be a compiled Java class file (`Client.class`) that has been misnamed. It contains the client logic.

## How to Run

Because `Server.java` and `Client.java` are likely compiled class files, you'll need to rename them before you can compile and run the application.

1.  **Rename the files:**

    ```bash
    mv Server.java test/Server.class
    mv Client.java test/Client.class
    ```
    *Note: The `Boot.java` file specifies the package as `test`, so the class files should reside within a `test` directory.*

2.  **Compile `Boot.java`:**

    You will need a Java Development Kit (JDK) installed.

    ```bash
    javac Boot.java
    ```

3.  **Run the application:**

    ```bash
    java test.Boot
    ```

This will start the server and then the client, which will connect to the server.
