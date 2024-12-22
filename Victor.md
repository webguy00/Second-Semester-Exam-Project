![Screenshot 2024-12-18 at 00-09-16 My Bio](https://github.com/user-attachments/assets/cdca075e-fe9c-4135-84f0-1ca44c0f5ac2)
https://34.245.212.137/
First of all i created an EC2 Instance,i gave my EC2 instance a name, then i selected ubuntu as my AMI, for my instance type i selected the default t2.micro instance type, which offers 1 vCPU and 1 GiB memory, and i created a new key-pair.
for the network setting i checked the boxes for, Allow SSH traffic from Anywhere, Allow HTTPS traffic from the Internet, and Allow HTTP traffic from the Internet. Then i launch my instance, after launching my instance, i connected to my instance and open my ubuntu terminal.
To create an Nginx server in my EC2 instance. I run the following commands in my Ubuntu terminal, Sudo -i, After logging in as the root user, i use these commands to update the package index and install NGINX in my system, sudo apt-get update, sudo apt install nginx, Next, i check the status of the Nginx with this command, service nginx status
To view the default webpage hosted by the NGINX server,i copy the Public IP address of my EC2 instance and paste it into my web browser.
To serve my static website,i replace the HTML code on the index page of the NGINX server with my own website’s HTML code.
To find the index webpage in the NGINX server,i navigate to the /var/www/html directory and list the files located there using this command, cd  /var/www/html/, ls
In this directory,i see the index.nginx-debian.html file, which is the index page of the NGINX server. To view the content of this file, i run the following command, cat index.nginx-debian.html
The next step i replace the HTML code in the index.nginx-debian.html file with the HTML code of my static website.
To do this, i open the index.nginx-debian.html file with nano editor, nano index.nginx-debian.html
Next,i use the arrow keys to navigate and edit the file. When i was done with the edits,i press Ctrl + O to save the file.
To exit Nano, i press Ctrl + X.

i refresh my Public IP page in my web browser to see my static website.
Congratulations to me,i have successfully deployed my static website on an AWS EC2 instance using NGINX.
