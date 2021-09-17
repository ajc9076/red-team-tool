# red-team-tool
Homework 3 - Red Team Tool - CDT 473

This tool is used to establish persistance on a Linux target after obtaining sudo/root priveleges.
All you have to do is drop the script on the machine and run it once using "sudo ./sys1og" and it will do the rest.

Persistance is established through SSH where you log in as "systemd-misc" with the password "systemd123".
The script also scrubs logs relating to the backdoor user's login in /var/log/auth.log.
A final step is that the backdoor user and their permissions get reset every 5 minutes by a cron job. 
