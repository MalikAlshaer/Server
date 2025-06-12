Basic server with threadpool

To host on your internet connection, comment the first line in the main function, and uncomment the line beneath

To host globally, open port 7878 (or whatever other port you would like, specified after ip address on the first line in the main function) using the following command:

For systems using ufw
"""sudo ufw allow 7878/tcp"""

for systems using iptables:
"""sudo iptables -A INPUT -p tcp --dport 7878 -j ACCEPT"""

To access the server from any other machine, insert your ip address into the browser followed by a colon and the port number. For example
"""1.2.3.4:7878"""

Also don't forget to open the port from the router using port forwarding.
