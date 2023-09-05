# velocity-web
host a HTML website on ec2

How to get the application code on ther ec2

-lauch an ec2 instance
-create a key pair 
- create security group and open port 22 and 80
-install software

- sudo su
- yum update -y
- yum install httpd -y (this is the virtual server we are using to install our software
- cd/var/www/html
-wget https://github.com/alexiangwa/velocity-web/archive/refs/heads/main.zip
- unzip main.zip
- cp -r velocity-web-main/* /var/www/html/
- rm -rf velocity-web-main main.zip velocity-html
- systemctl enable httpd
- systemctl start httpd
