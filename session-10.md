# Package Management In Linux 

    What is a package ? Package is noting but a software.
    Linux as a kernal + os comes very basic, based on your needs we are going to install the needed packages on the system.
    Like any other system, even linux get updates very frequently. So, as per the org policy we need to patch / update them on a monthly / quarterly basis.

    What is need of an update to an OS or Software or Update ? 
        > Update brings you additional feature and strenghten's the software.
        > Pathces sometimes offer better performance.
    
    How to update or what are the package management tools on linux ?

        yum , dnf,     ( Redhat / Centos )
        apt , apt-get  ( Ubuntu)

        Redhat 7 , YUM is the package managed
        From Redhat 8, YUM & DNF ( dnf is the latest package manager )

> sudo yum list installed : Shows the packages thar are installed on the server
> sudo yum list available : Shows the packages thar are available in the interner for our particular OS
> How to install , remove or update a package ?

```
    # yum install packageName or dnf install packageName 
    $ yum remove packageName or  dnf remove packageName
    $ yum update packageName or dnf update packageName
    $ sudo dnf update --exclude=java* 
    $ sudo dnf update --exclude=kernel*
    How to search for the available versions ?
     $ sudo dnf search openjdk
     $ sudo dnf install java-1.8.0-openjdk
    Installing packages from file with the packageNames mentioned
     $ sudo dnf install $(cat package.txt)
    
```
Packages on redghat linux can be installed in 3 ways 

    1) Package Manager ( yum or dns ) : Along with the needed package, all the pre-requisites are covered by the package manager 
    2) RPM Files ( Downthe rpm's and install them): You're responsible for all the packages that are needed for the package you're installing
    3) Code Baesd installation ( npm install , go mod ) 

> Service Management

    Job: A job is nothing but a task, that runs and goes for a completion. 
    Service: This is nothing but a process that continuously waits for some task, even after the completion of the process, it still waits for the next process. 
        Example: ssh, ftp, smtp
    
    # systemctl status serviceName
    # systemctl stop serviceName
    # systemctl restart serviceName
    # systemctl daemon-reload
    # systemctl list-units -t service
    # netstat -tulpn

> Future Scope
Our machine's won't have public ip
you cannot access or ssh these vm's from Internet
But these machines can talk to the Internet ( NAT )