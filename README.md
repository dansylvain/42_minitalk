# Minitalk Project Documentation
Utilizing Unix signals for efficient process communication.
## Introduction
The "minitalk" project is a small client-server application implemented in C, allowing for communication between two processes using signals. It provides a simple and efficient way to exchange messages between a client and a server in a Unix-based environment.

In the "minitalk" application, one process acts as the server, while the other process acts as the client. The client sends messages to the server, which receives and displays them. The communication between the client and server is achieved through the use of signals, specifically the SIGUSR1 and SIGUSR2 signals.

The primary goal of the "minitalk" project is to demonstrate inter-process communication (IPC) using signals in Unix systems. It serves as a practical example of how signals can be used to establish communication channels between processes, enabling lightweight and efficient message passing.

Through this project, users can gain a deeper understanding of signal handling and IPC mechanisms in Unix-based operating systems, as well as enhance their skills in network programming and system-level development.
## Execution
### Cloning the Repository
To use the "minitalk" application in your project, clone the repository containing the necessary files from GitHub:

```bash
git clone <https://github.com/dansylvain/42_minitalk>
```
### Compiling the Program
Navigate to the project directory and compile the client and server programs using the Makefile:
```bash
cd minitalk
make
```
### Running the Programs
Once compiled successfully, you can run the client and server programs. Start the server program first, followed by the client program. Here's how to do it:<br>
* **Start the server:**
```bash
./server
```
The server will start and display its pid. You need it for the next step.<br>
* **In a separate terminal window, run the client:**
```bash
./client <server_pid> <message>
```
Replace <server_pid> with the process ID of the server (displayed when you start the server), and <message> with the message you want to send to the server.

## Dependencies
My implementation of the "philosophers" project includes all necessary dependencies within the source code, requiring no additional installations.
