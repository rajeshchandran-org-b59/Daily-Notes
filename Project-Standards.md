1) Using Lab AMI, we will provision "t3.micro" spot VM's ( without keyPair )
2) They are expected to have "B59-Sg" [ A security group that allows all ports from the internet ]
3) Each and every VM is expected to have the Application Component Name.

    AMI To Use  : DevOps-LabImage-RHEL9
    Region      : N.Virginia
    Credentials : ec2-user/DevOps321

Make sure you provison a VM ( On Demand! Not spot ) and name is as WS or Workstation using the above LAB AMI.
This WS is something, we are going to use to install and test all the basic needs and this will be lasting till the end of the training.



Terminal is just an entry point;
But installing GitBash, your terminal has the capability to run the git commands 

Non-Functional Requirements ( NFR )
Code Should Be Dry 
Credentials should not be hardcoded.
Re-run of the script should not fail.