# kamhost
KaM Remake Dedicated Server Init.d service script

Make a KaM Dedicated Server a System Service on Ubuntu

1. Place your dedicated server files in /etc/KaMHost (or your can place it elsewhere and change the path in KaMHost file)

2. Edit KaMHost file:
    *. In "SCRIPT=...", Change "/etc/KaMHost" to your own path
    *. If you use 32 bits version, remove "_64" from the end of that line
    *. In "RUNAS=root" change root for another user (executing as root is dangerous!). The user should have full permision on the SCRIPT path, also on PIDFILE and LOGFILE path (you can change them)

3. Copy KaMHost to /etc/init.d/KaMHost

4. sudo chmod +x /etc/init.d/KaMHost

5. sudo systemctl daemon-reload

6. sudo service KaMHost start

7. Check the status with sudo service KaMHost status

This script was made for my project Nostalgia-Gamers.com

KaM Remake Website: http://www.kamremake.com/

Kam Dedicated Server Downloads: http://www.kamremake.com/download/
