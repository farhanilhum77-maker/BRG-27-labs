# BRG-27-labs


Setting Up Linux

In this lab, the first step that I learnt was how to set up GitHub. This is the first time I am using GitHub and created a repository. I had trouble understanding how GitHub works and what it is for. Eventually, I was able to set up GitHub locally at my laptop and share my GitHub link to the professor. 

Next, I installed Ubuntu Linux both Desktop and Server iso file using VirtualBox to simulate real server environment. I faced difficulty understanding how virtual machines allocate resources such as RAM and storage. However, after configuring the virtual machine with 20GB disk space and 4GB RAM, I successfully installed Ubuntu.


Exploring Linux

After installing Ubuntu, I explored basic Linux commands like cd, pwd, ls, mkdir and many more. It was challenging for me to navigate without any graphical user interface at first but after some practice, I got the hang of it. 
I also learned about the Linux directory structure like /home, var which are important for system configuration and logging. Using the “man” command helped me understand how to independently learn commands. I have also learnt to press “q” to stop viewing long output.
All these exercises gave me confidence in using CLI tool, which is essential when learning about server environments where GUI are usually not available.
 

Managing and controlling Linux

In this session, I was taught on how to manage system services using the command “systemctl”. I practiced listing services, check their status, start or stop them. I also learnt how to install missing services such as SSH that was not found in my Ubuntu even after using the “sudo apt update” and “sudo apt upgrade -y” command. I was able to install the ssh services using the command “sudo apt install openssh-server -y“ and “sudo systemctl enable --now ssh”. Now I am able to check the status of the SSH services on my Ubuntu Linux. This skill is important for troubleshooting servers, as many issues are related to services not running correctly.


Understanding and applying linux

I explored file permissions using ls -l, chmod, and chown. Initially, I found permission values like 755 confusing but after learning that they represent read, write, and execute access, it became clearer. 
I created a new user using “adduser” command and then added a new group by using “addgroup”. Afterwards, I used the chown command to change owner of “file.txt”. This lab highlighted the importance of access control in security. Incorrect permissions can lead to unauthorized access or system vulnerabilities.


Searching and Navigating the Linux File System

I used commands such as find and grep to locate files and search content. These tools were very powerful but required precise syntax. Below screenshot shows that I used “grep” command to find the word “text” from the home folder.
I realised that these commands are extremely useful in real-world scenarios, such as searching logs or troubleshooting issues in large systems.
This improved my efficiency in navigating systems and finding information quickly.


Total Cost of Ownership (TCO) in Cloud Infrastructure

In this lab, I compared cloud services with on-premise infrastructure using Excel. I calculated costs such as hardware, maintenance, and subscription fees. I learned that while cloud services have ongoing costs, they reduce upfront investment and maintenance effort. This activity helped me understand decision-making in IT environments, where cost and scalability are key considerations. This lab is highly relevant to real-world IT roles such as system administrators and cloud engineers, where cost optimization and infrastructure planning are critical. Understanding TCO allows organizations to make informed decisions based on both financial and operational factors.


Provisioning and Securing a Cloud VM (AWS EC2)

I launched an Ubuntu instance on AWS EC2 and connected to it using SSH. Initially, I had difficulty understanding key pairs and security groups. I had to redo the instance part as I got confused. It took me a while but eventually I was able to configure the instance and connect to the instance via SSH in Ubuntu Linux. I also updated the system using apt update and apt upgrade. This lab provided real-world experience in cloud deployment, which is widely used in modern IT infrastructure.
 

Writing Bash Scripts and Using Regular Expressions

I created a basic Bash script to automate simple tasks. I created a simple “Hello Server” script whenever I execute the script. This simple command and script has given me more confidence when it comes to doing scripts.


Configuring DNS and Testing Domain Resolution

I configured DNS by linking a domain to my server’s IP address and tested it using nslookup and dig. This lab helped me understand how domain names are translated into IP addresses, which is essential for web services. DNS is a critical component of networking, and misconfiguration can lead to service downtime. I used DuckDNS as an example. I used Apache to secure the server.

