Basic server with threadpool

To host locally  on your internet connection, follow instructions in the main function in src/main.rs.

To host globally, open port 7878 (or whatever other port you would like, specified after ip address on the first line in the main function) using the following command (replace 7878 with the whatever port if changed):

For systems using ufw:
```
sudo ufw allow 7878/tcp
```

For systems using iptables:
```
sudo iptables -A INPUT -p tcp --dport 7878 -j ACCEPT
```

To access the server from any other machine, insert your ip address into the browser followed by a colon and the port number. For example:
```
1.2.3.4:7878
```

For this to work it is important to open the port from the router with port forwarding.
