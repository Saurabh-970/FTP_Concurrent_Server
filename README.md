#🚀 Overview
The server waits for incoming connections.
The client connects to the server and requests a file.
The server sends:
 1 File size (header)
 2 File data (in chunks)
The client receives and saves the file locally.

#⚙️ Technologies Used
C Programming
TCP/IP Sockets
Linux System Calls (socket, bind, listen, accept, connect, read, write)
File Handling (open, read, write)

#🔄 Workflow (Step-by-Step)
1. Server Initialization
  1 Creates a TCP socket
  2 Binds it to the given port
  3 Starts listening for client requests
   
2. Client Connection
    Client creates socket
    Connects to server using IP and port
   
3. File Request
    Client sends the file name (e.g., Demo.txt)
   
5. Server Processing
    Server reads the requested file
    Sends header:
