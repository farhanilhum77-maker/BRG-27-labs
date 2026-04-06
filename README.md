# BRG-27-labs

Installing a Linux Environment on My PC

In this lab, the first step that I learnt was how to set up GitHub. This is the first time I am using GitHub and created a repository. I had trouble understanding how GitHub works and what it is for. I had no idea on how to edit my repository and the README file. Eventually, after research, I was able to set up GitHub locally at my laptop and share my GitHub link to the professor. 

Next, I installed Ubuntu Linux both Desktop and Server iso file using VirtualBox to simulate real server environment. I faced difficulty understanding how virtual machines allocate resources such as RAM and storage. However, after configuring the virtual machine with 20GB disk space and 4GB RAM, I successfully installed Ubuntu.

   
Exploring Ubuntu Desktop and CLI Tools

After installing Ubuntu, I explored basic Linux commands like cd, pwd, ls, mkdir and many more. It was challenging for me to navigate without any graphical user interface at first but after some practice, I got the hang of it. 

I also learned about the Linux directory structure like /home, var which are important for system configuration and logging. Using the “man” command helped me understand how to independently learn commands. I have also learnt to press “q” to stop viewing long output.
All these exercises gave me confidence in using CLI tool, which is essential when learning about server environments where GUI are usually not available.
 

Managing and controlling Linux Services

In this session, I was taught on how to manage system services using the command “systemctl”. I practiced listing services, check their status, start or stop them. I also learnt how to install missing services such as SSH that was not found in my Ubuntu even after using the “sudo apt update” and “sudo apt upgrade -y” command. I was able to install the ssh services using the command “sudo apt install openssh-server -y“ and “sudo systemctl enable --now ssh”. Now I am able to check the status of the SSH services on my Ubuntu Linux. This skill is important for troubleshooting servers, as many issues are related to services not running correctly.

 
Understanding and applying linux permissions

I explored file permissions using ls -l, chmod, and chown. Initially, I found permission values like 755 confusing but after learning that they represent read, write, and execute access, it became clearer. 
I created a new user using “adduser” command and then added a new group by using “addgroup”. Afterwards, I used the chown command to change owner of “file.txt”. This lab highlighted the importance of access control in security. Incorrect permissions can lead to unauthorized access or system vulnerabilities.

 
Searching and Navigating the Linux File System

I used commands such as find and grep to locate files and search content. These tools were very powerful but required precise syntax. Below screenshot shows that I used “grep” command to find the word “text” from the home folder. I realised that these commands are extremely useful in real-world scenarios, such as searching logs or troubleshooting issues in large systems. This improved my efficiency in navigating systems and finding information quickly.

 
Total Cost of Ownership (TCO) in Cloud Infrastructure

In this lab, I compared cloud services with on-premise infrastructure using Excel. I calculated costs such as hardware, maintenance, and subscription fees. I learned that while cloud services have ongoing costs, they reduce upfront investment and maintenance effort. This activity helped me understand decision-making in IT environments, where cost and scalability are key considerations. This lab is highly relevant to real-world IT roles such as system administrators and cloud engineers, where cost optimization and infrastructure planning are critical. Understanding TCO allows organizations to make informed decisions based on both financial and operational factors.

 
Provisioning and Securing a Cloud VM (AWS EC2)

I launched an Ubuntu instance on AWS EC2 and connected to it using SSH. Initially, I had difficulty understanding key pairs and security groups. I had to redo the instance part as it was too confusing. It took me a while but eventually I was able to configure the instance and connect to the instance via SSH in Ubuntu Linux. I also updated the system using apt update and apt upgrade. By doing this lab, provided real-world experience in cloud deployment, which is widely used in modern IT infrastructure.
 

Writing Bash Scripts and Using Regular Expressions

I created a basic Bash script to automate simple tasks. I created a simple “Hello Server” script whenever I execute the script. This simple command and script have given me more confidence when it comes to doing scripts.

 
Configuring DNS and Testing Domain Resolution

I configured DNS by linking a domain to my server’s IP address and tested it using nslookup and dig.  I used DuckDNS as my domain. This lab gave me the hardest time as I was unable to get my web server to be working. I found out it is due to my port 80 to be connected to Apache instead of Nginx. 
This error helped me to learn on how to troubleshoot if that is the case which is by removing the apache clean from the server then enabling back the nginx services. I also missed the part where I have to add in the inbound rules for HTTP and HTTPS. This has caused me a lot of time troubleshooting the error. Additionally, I also added in the wrong security group for the HTTP and HTTPS. But eventually, I was able to troubleshoot and enter my domain using the browser

This lab helped me understand how domain names are translated into IP addresses, which is essential for web services. DNS is a critical component of networking, and misconfiguration can lead to service downtime. 


Obtaining and Managing Digital Certificates with Let’s Encrypt

I installed Certbot and generated an SSL certificate for my server. I verified HTTPS access through the browser. I was unable to complete this the first time as there was an issue with my DNS server previously. After troubleshooting my DNS server, I was able to complete this section quite smoothly. I was able to secure my server from HTTP to HTTPS.

This lab emphasized the importance of encryption in protecting data during transmission.
This is especially relevant in cybersecurity, where securing communication channels is essential.

 
Scripting Linux Server Functions for Automation

I created a simple script to automate tasks such as echo Hello World. This lab showed me on how to write a script using the nano command and changing the permission and allowing it to be executed using the “chmod +x” command. I then execute the command running the “./script.sh” command. This opens up a lot of possibilities for me to play around in the future if I want to created much more complicated scripts.

 
Additional Server Service: Docker

I installed Docker and ran a test container. This was my first experience with containerisation. I had trouble understanding what containerisation is even after researching about it. But thanks to this lab, I am able to understand much more clearly about Docker. I installed the docker software then start the services using the “systemctl start docker” command. I then enable the docker to start with my experiment. I learned online on how to containerise my nginx but using the command “sudo docker run -d -p 8080:80 nginx”.

Thanks to this, I learned that Docker allows applications to run in isolated environments, making deployment faster and more consistent. This is widely used in DevOps and cloud environments.
 

Overall Reflection

Overall, I gained valuable hands-on experience in setting up and managing server environments across both local and cloud platforms. At the beginning, I found the transition from a graphical interface to a command-line environment challenging, especially when working with Linux commands and system configurations. However, as I progressed through the sessions, I became more confident in navigating the system, managing services, and troubleshooting issues independently.

One of the most significant learning experiences was deploying and configuring a cloud-based server using AWS. This allowed me to understand how real-world infrastructure is provisioned and secured. Configuring DNS using DuckDNS and implementing SSL certificates with Let’s Encrypt further enhanced my understanding of how web services are made accessible and secure. I also encountered practical issues such as service conflicts and incorrect security group settings, which required systematic troubleshooting. These challenges improved my problem-solving skills and reinforced the importance of attention to detail.

The automation tasks using Bash scripting demonstrated how repetitive administrative tasks can be streamlined, increasing efficiency and reducing human error. Additionally, installing Docker introduced me to containerisation, which is widely used in modern DevOps practices for scalable and consistent deployments.

Overall, this learning journey has strengthened my foundational knowledge in system administration, cloud computing, and security. It has also given me insight into real-world IT roles such as system administrators, DevOps engineers, and cybersecurity professionals. I now have a clearer understanding of how different components such as networking, automation, and security work together to support a reliable and secure server environment.
