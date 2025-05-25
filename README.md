# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

PROGRAM

CLIANT
`import socket 
from pythonping import ping 
s=socket.socket() 
s.bind(('localhost'8000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
hostname=c.recv(1024).decode() 
try: 
c.send(str(ping(hostname, verbose=False)).encode()) 
except KeyError: 
c.send("Not Found".encode())``

```

SERVER
```
 import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
ip=input("Enter the website you want to ping ") 
s.send(ip.encode()) 
print(s.recv(1024).decode())
```


## Output
```
![Screenshot 2025-05-25 205904](https://github.com/user-attachments/assets/6690ba70-0701-41ff-aedb-d5aadd0e92a8)
```
```
![Screenshot 2025-05-25 205914](https://github.com/user-attachments/assets/8c259b6a-ec7f-4035-9d85-3551c3ad7b84)
```
```
![Screenshot 2025-05-25 205933](https://github.com/user-attachments/assets/fda22fb8-bfc8-4baa-b042-94918a38b697)
```
```
![Screenshot 2025-05-25 205942](https://github.com/user-attachments/assets/1a1e8b25-ee3d-4795-814b-9e00b42ffe4a)
```
```
![Screenshot 2025-05-25 205949](https://github.com/user-attachments/assets/a77a97a6-8e18-43e7-b2b7-5b6e4a518c24)
```
```
![Screenshot 2025-05-25 205956](https://github.com/user-attachments/assets/97fa3b3f-1012-4fb4-ab31-34aa113f5a3a)
```
```
![Screenshot 2025-05-25 210005](https://github.com/user-attachments/assets/590d1aee-2278-40ab-a4ab-8d487e13f855)
```
```
![Screenshot 2025-05-25 210014](https://github.com/user-attachments/assets/8c3163c5-44ca-42ba-b475-d2ff99f1c972)

```

## Result
Thus Execution of Network commands Performed 
