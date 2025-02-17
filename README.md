# Web Server:
This is a basic HTTP server written in Python 3.7+ using the socket module. It listens on port 8888 and responds with a simple HTTP message.

### 1️⃣ Prerequisites:
Python 3.7 or higher
A terminal or command prompt

### 2️⃣ Run the Server:
Copy and save the script as server.py, then run:

python server.py
You should see:

Serving HTTP on port 8888 ...

### 3️⃣ Access the Server:
Open a browser and go to:

http://localhost:8888
Or use curl in the terminal:

curl http://localhost:8888

### 4️⃣ Expected Output:
The server will return:

Hi there, My name is Amna! And I am just a coder like you.
The request details will also be printed in the console.

# 🛠 Code Explanation:
1️⃣ Creates a TCP socket using socket.AF_INET, socket.SOCK_STREAM.
2️⃣ Binds to HOST (empty string) and PORT (8888) → Accepts connections on all available network interfaces.
3️⃣ Listens for incoming connections (listen_socket.listen(1)).
4️⃣ Accepts client requests, reads HTTP request data, and prints it.
5️⃣ Sends an HTTP response with HTTP/1.1 200 OK.
6️⃣ Closes the connection to handle the next request.

