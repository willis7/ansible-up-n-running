# Some useful commands

To check the uptime of our server
`$ ansible testserver -m command -a uptime`

Command module is default so this is also valid:
`$ ansible testserver -a uptime`

Commands with spaces:
`$ ansible testserver -a "tail /var/log/dmesg"`

Commands as sudo:
`$ ansible testserver -s -a "tail /var/log/syslog"`