# red-team-tool
Red Team Tools - CDT 473

Suite of tools I developed for the 3rd competition. 

- sys1og: establish persistance on a Linux target after obtaining sudo/root priveleges.
All you have to do is drop the script on the machine and run it once using "sudo ./sys1og" and it will do the rest.
Persistance is established through SSH where you log in as "ssh" with the password "sshuser123".
The script also scrubs logs in /var/log/secure and /var/log/syslog.
A final step is that the backdoor user and their permissions get reinstated every 5 minutes by a cron job. 

- user-spraying: create 100 users with the creds: LOLGETREKT#:LOLGETREKT# where # is 0 to 100. LOLGETREKT0 should have system.
Run by using "sudo ./user-spraying". 

- permission-nuke: chmod 777 to most folders allowing even standard users to access many files. Also attempted to set umask but might not work.
