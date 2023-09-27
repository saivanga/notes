Daemon
Processes = Instance of a running program

ps -aux
* Lists all the processes

ps -aux | grep sublime
* Lists all the processes which contains the name - sublime

* Every time we open any program - One/multiple processes will start for that program
* Once we close that program - Related processes will be stoppe automatically

Daemons are the processes that we don't start
They are like background processes
Can also be referred as services

Every daemon file will contain a `d` at the end.
Example daemons:
