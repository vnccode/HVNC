# HVNC
HVNC , hidden remote VNC desktop with backconnect


- Direct  mode ( tvnviewer.exe launched on Windows VPS)

Run tvnviewer.exe

click listen mode ( port 5500)

Run  builder.exe

Enter VNC  server IP


- Tunnel mode (tvnviewer.exe behind a router , firewall)

Linux  VPS 

Edit ssh config 

sudo nano /etc/ssh/sshd_config 

Inside the sshd_config file  change the #PermitTunnel setting from no to yes.

PermitTunnel yes

and GatewayPorts yes

sudo reboot

Windows

run tvnviewer.exe

click listen mode ( port 5500)

edit tunnel.bat change VPS IP and password

run tunnel.bat

Press return to begin session

Run  builder.exe

enter VPS IP

build.exe will periodically connect to your vncviewer.exe server

For reconnect remove desktop name from r.txt file

contact cyy374h@outlook.com


