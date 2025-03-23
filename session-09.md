Agenda: 
    * Run Levels in linux 
    * Process Management In linux 
    * Network management in linux 
    * User Managment 
    * Permissions 
    * Patch Management 
    * Service Management

Run Level in linux: 
    0 : Shutdown's the server 
    1 : Starts the server in a single user mode 
    2 : Starts the server in multi-user mode but network ( nfs ) won't be coming 
    3 : This starts the system in multi-user mode with network ( Efficient and widely used )
    4 : This is for R&D, not for users purpose. 
    5 : This also starts your server in a multi-user mode, but starts the server along with GUI
    6 : Reboot

$ df -h 
$ df -Th
$ du -h fileName

> Pipes ( | ):
    Pipes helps in converting the output of first command as an input to the second command 

        $ ls -ltr | grep passwd

> sudo: gives the user temporary root privileges to execute the specific command as a root user.

> Process Management:
    All the actions would be running in the backend as a process which does the job.

$ top   //This is a task manager like interactive mention, we won't use
$ ps   //This is not an interactive but the result is static and are related only to that session
$ ps -e   //Shows every process in the system
$ ps -ef  //In detailed process
$ ps -u   //process associated with current user only

> Load Average
    `Ex: load average: 0.07, 0.05, 0.02`
    In Linux, "load average" refers to a metric that indicates the average number of processes that are either currently running on the CPU or waiting to be executed, essentially showing how heavily the CPU is being utilized over a specific period of time (usually 1, 5, and 15 minutes). 

$ kill: command to kill a specific process id 
    $ kill pID     [ Will terminate the process by updating the system ]
    $ kill -9 pID  [ Forcefull kills a process ]

> User Management: 
    By default each and every will be part of his own group 
    We can create a maximum of 65535 users on a linux server
    root is the first user account created on the linux server
    Each and every user in linux will have a UID and root user's uid is 0

    AAA
        Authentication 
        Authorization
        Auditing
    
    How to create a user account ?
    What is a group account ?
    How to create a group account ?
    How to add a user to a group account ?
    How can groups can a user be a part ?

> How to switch from one user account to another user account ?
    su: switch user
    su - : switch user along with this directory

> Not everyone is the system can execute the commands with `sudo` !!!!!
    How can we give a specific group permissions to sudo ?
        /etc/sudoer
        devops : createUser accounts ( for sudo )
        