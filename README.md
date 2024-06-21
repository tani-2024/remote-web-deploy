# Web Deployment Automation Project
Here we see the power of scripting! We can automate our daily tasks by writing scripts and executing them. 
In this project, I set up a Tooplate website on client machines by writing scripts on a control machine.

**Overview**
This project demonstrates how to automate the deployment of a website on multiple remote machines (clients) using Bash scripts. 
The control machine is a CentOS VM, while the client machines include one Ubuntu VM and one CentOS VM

**Steps**
1. Bring Up All Three VMs
Ensure that all three virtual machines (one control and two clients) are up and running.

2. Update /etc/hosts File
Add the IP addresses and hostnames of the remote machines to the /etc/hosts file on the control machine for easy SSH access.

3. Create a 'devops' User on Client Machines
Create a devops user on both client machines and add it to the sudoers list using the visudo command.

4. Generate SSH Keys
Generate SSH keys on the control machine and copy the private key to the client machines using the ssh-copy-id command.

6. Create remohosts File
Write a remohosts file that contains the hostnames of all remote machines. This file will be used to iterate over all client machines in the deployment script.

6. Write the Web Setup Script
Create a script (websetup.sh) to set up the website on remote machines for both Ubuntu and CentOS.

7. Write webdeploy.sh Script
Write the webdeploy.sh script, which will set up the website on all remote machines listed in the remohosts file.

8. Access the Website
Now, you can access the deployed website using your browser. Navigate to the IP address or hostname of your client machines.
