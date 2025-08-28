# AWS LEMP STACK ON AWS EC2 
This project is to use LEMP Stack to set-up and configure the following: 
A. Linux server - Ubuntu
B. Nginx for  Web server (http)
C. MySql - Database
D. Php - for dynamic pages
## 1. Creating AWS Instance
1. I created an Instacne in AWS and named it Ubuntu-LAMP
2. I chose Ubuntu from list of servers
3. The configuration is 24.04 amd noble, 64-bit, t2.micro free tier, 8 Gig storage
4. I opened http and ssh ports; and allowed traffic from anywhere
5. I created a .pem key to connect to the server 
![alt text](LEMP/AWSinstance.PNG)
## Connecting to AWS Instance (Ubuntu Server)
1. I run ssh-i command to connect to the server using the public ip address 
![alt text](LEMP/sshconnect.PNG)
## Installing Nginx Web server
In order to serve web pages to visitors I will install Nginx which is a high performing web server
1. I updated and upgrade the list of packages in the package manager using (sudo apt update && sudo apt upgrade)
![alt text](LEMP/Ubuntu_update.PNG)   
2. I installed Nginx server using the sudo apt install 
![alt text](LEMP/Nginx_install.PNG)  
3. I enabled Nginx after installation using systemctl enable
4. I connect to the apache server through localhost using curl command
![alt text](LEMP/curl_localhost.PNG)
5. I connect to the Nginx server using 127.0.0.1:80
![alt text](LEMP/curl_localhost_ip.PNG)
6. I coonect to the Nginx server through web browser
![alt text](LEMP/Nginx_webpage.PNG)

   