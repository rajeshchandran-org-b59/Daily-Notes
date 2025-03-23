# Linux Basics 

Connection Timeout vs  Connection Refused 

Timeout: Firewall is stopping the request
Refused: Request is received at the server, but server is rejecting the request

Vertical Scaling: Means adding resources to the same server. Vertical Scaling always involves downtime.

cd vs pwd 

cd ..  ( move one step back )
pwd : displays present working directory

# mkdir dirName


Servers are created to run applications.
Servers will be accessed by Developers, QA, DevOps, SecOps, Seucity Team from the company 
Each and every user need to have an account in the system.

In linux, `root` is the first user account creates in the system and the ID of it 0
We can create a maximum of 65535 user accounts and out which 0 to 999 are system accounts, created and managed by system for a specific job.

# cat vs tac 

> Use Cases of reading file: 
1) Reading the file.
2) Reading file in the reverse order.
3) How to read from the top 5 lines of a file.
4) How to read from the bottom 5 lines of a file.
5) How to read the file from line 5 to 8.
6) How to read a specific portion or fields of a file.
7) How to print line number x and y 

# head & tail 
> head reads the top 10 lines of a file
> tail reads the last 10 lines of a file 

# sed : streamline editor
    `$ sed -n -e '8,13 p' /etc/passwd`
    `$ sed -n -e '2 p' -e '5 p' /etc/passwd`

# cut: field separator tool
    `cut -d : -f1 /etc/passwd`
# Prints field 1 and 4 from the mentioned file with : as delimited
    `$ cut -d : -f1,4 /etc/passwd`
# prints 1 to 4 fields from the file:
    `$ cut -d : -f1-4 /etc/passwd`

# How to read, cp, rm, mv of a file. How to edit a file ?
vi fileName 
vim fileName

> Editing a file on linux starts with understand the modes of editor.

w: write ( save )
q: quit 
wq! : Save and quit 

> When you write something on the file, but don't want to save it and in this case,
:q!

# Directory Structure In Linux

# curl: client url : Like a Browser on linux
    using curl, you can read / download files from the internet.
    `$ curl url`

# wget: to download files from the internet 
    `$ wget URL`

>  Tar, pipe, patching & user management on linux...