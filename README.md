# LockNote

Welcome to **LockNote**, the next-generation solution for secure conversations. Built with multiple layers of encryption on the robust Python ecosystem, **LockNote** ensures that your conversations remain private, protected, and uncompromised.

Whether you're handling sensitive business information or simply chatting with friends, **LockNote** guarantees the highest levels of security through cutting-edge encryption technology. By prioritizing user privacy and data protection, we bring you a platform that keeps your communications secure from unauthorized access.

## Features of LockNote

1. **End-to-End Encryption**  
   All messages are encrypted from the sender to the receiver, ensuring that no one in between can access your conversations.

2. **User-Friendly Interface**  
   The simple, intuitive design makes it easy for users to navigate and communicate.

3. **Multi-Platform Support**  
   Whether you are using a desktop or a mobile device, **LockNote** is always accessible.

4. **Robust Backend**  
   Powered by Python, **LockNote** ensures fast and reliable communication.

5. **Open Source**  
   Access our codebase, contribute, and help improve the system.

6. **Group Chats**  
   Have encrypted group conversations with multiple participants, keeping all messages secure.

7. **Adaptive Encryption Modes**  
   Switch between encrypted and unencrypted chat modes based on your specific needs.

8. **Direct Messaging (DM)**  
   Message individual users privately with end-to-end encryption.

## Requirements

To use **LockNote**, ensure the following dependencies are installed:

- **Python 3.x**
- **cryptography library**
- **colorama library**

To install the required packages, run:

```bash
pip install cryptography colorama
```

## Usage

### Unencrypted Mode

Run the server and client applications in unencrypted mode as follows:

**Server:**

```bash
python3 server.py --help
```

**Example usage:**

```bash
python3 server.py --host 0.0.0.0 --port 12345 --loglevel INFO --logfile server.log
```

**Client:**

```bash
python3 client.py --help
```

**Example usage:**

```bash
python3 client.py --host 127.0.0.1 --port 12345
```

### Encrypted Mode

Use the encrypted mode of **LockNote** for added security:

**Server (Encrypted):**

```bash
python3 serverE.py --help
```

**Example usage:**

```bash
python3 serverE.py --host 0.0.0.0 --port 12345 --key mysecretpassword --loglevel INFO --logfile server.log
```

**Client (Encrypted):**

```bash
python3 clientE.py --help
```

**Example usage:**

```bash
python3 clientE.py --host 127.0.0.1 --port 12345 --key mysecretpassword
```

### In-Program Help Menu

Once connected, users can access the help menu for a list of commands:

**Help Menu:**

- `/help` &rarr; Display the help menu.
- `/exit` &rarr; Exit the program.
- `/clear` &rarr; Clear the chat screen.
- `/userlist` &rarr; View the list of connected users.
- `/dm [user] [message]` &rarr; Send a direct message to a user.
- `/changeuser [new_username]` &rarr; Change your username.

### Command Line Options Summary

| Command Option | Description                                       |
|----------------|---------------------------------------------------|
| `--help`       | Show help message and exit.                       |
| `--host`       | IP address to bind the server/client.             |
| `--port`       | Port number for the server/client.                |
| `--key`        | Secret key for encryption (for encrypted mode).    |
| `--loglevel`   | Set logging level (`DEBUG`, `INFO`, `WARNING`, `ERROR`). |
| `--logfile`    | Specify the log file for logging output.           |

