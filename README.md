# HVNC
HVNC , hidden remote VNC desktop with backconnect

- Direct  mode

Run vncviewer.exe
click listen mode ( port 5500)

Run  builder.exe
Enter VNC  server IP

- Tunnel mode

Linux  VPS 

Edit ssh config 
sudo nano /etc/ssh/sshd_config
Inside the sshd_config file  change the #PermitTunnel setting from no to yes.
PermitTunnel yes
sudo reboot

Windows

run vncviewer.exe
click listen mode ( port 5500)
edit tunnel.bat change VPS IP and password
run tunnel.bat
Press return to begin session

Run  builder.exe
enter VPS IP

For reconnect remove desktop name from r.txt file

