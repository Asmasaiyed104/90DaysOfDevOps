# syslog is the standard protocol for message logging in computing.

It allows devices such as router, switches , firewall and servers to generate event message and send them to centralized server for storage , analysis and security.

# grep error /var/log/syslog 2>/dev/null

grep → search text
error → word to search
/var/log/syslog → log file being checked
2> → redirects errors
/dev/null → black hole in Linux (discards output)

# du -sh /var/log/\* 2>/dev/null | sort -h | tail -5

du -sh /var/log/\*
du → disk usage
-s → summary only
-h → human readable (K, M, G)
Shows size of each file/folder in /var/log

sort -h it will sort size

tail -5 shows the last 5 lines
useful for debugging disk full issue, cleaning old logs, monitoring server storage usage

# cat /etc/hostname

it will dispaly the sys ip(servername)

# ls -la ~

It shows all files and folders in your home directory, including hidden files, with detailed information.
ls listing file and folder
-l long listing formate (perminssion,owner,size date, filename) -a (shows hidden file )

# systemctl list-units nginx

It shows all active systemd units running on the Linux system.

# systemctl is-enabled nginx

Checks whether the nginx service starts automatically when the server boots.
