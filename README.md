# red-team-tool
Homework 3 - Red Team Tool - CDT 473

This tool is used to establish persistance on a Linux target after obtaining sudo/root priveleges.
All you have to do is drop the script on the machine and run it once using "sudo ./sys1og" and it will do the rest.

Persistance is established through SSH where you log in as "systemd-misc" with the password "systemd123".
The script also scrubs logs in /var/log/auth.log and /var/log/syslog.
A final step is that the backdoor user and their permissions get reinstated every 5 minutes by a cron job. 

This script is verified to work with a standard Ubuntu installation. 
