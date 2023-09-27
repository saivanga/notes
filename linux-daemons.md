Daemon
Processes = Instance of a running program

ps -aux
* Lists all the processes

ps -aux | grep sublime
* Lists all the processes which contains the name - sublime

* Every time we open any program - One/multiple processes will start for that program
* Once we close that program - Related processes will be stoppe automatically

Daemons are the processes that we don't start
* They are like background processes
* Can also be referred as services

Every daemon file will contain a `d` at the end.

Example daemons:
1. sshd
2. systemd
3. ntpd
4. httpd
   etc...

systemd - Boss of daemons - This controls daemons - starts/stops/restarts other daemons
* It is the first service/daemon that will be started after booting a linux system (boot -> kernel -> systemd)


Command
* pstree
Lists tree of daemons and we can see which daemon started other daemons.

Every process will have a process id.
We can see this process id when we use the command `ps -aux`
As systemd is the first daemon that will be started it will always contain the process id as `1`




