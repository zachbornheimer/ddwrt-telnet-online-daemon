# ddwrt-telnet-online-daemon
Reboot the router if it is no longer connected.

By Zachary Bornheimer
Where applicable, licensed under the GPLv3

The executive goal of this program is to have a cronjob run every 5 minutes that determines if the software is running.  If it isn't, it is started.

This is designed to get the software to determine if it is online by use of pinging ifconfig.co - it allows us to ensure the VPN is enabled as well.  If there is no response, it uses an expect script to log into the router and reboot it.

Required software:
xterm
perl5
gcc
expect
