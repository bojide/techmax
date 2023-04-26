Credit to AOS Note

Asset provided below:
How to Host a Website on an EC2 Instance

sudo su
yum update -y
yum install -y httpd
cd /var/www/html
wget https://github.com/azeezsalu/techmax/archive/refs/heads/main.zip (Make sure to change the name "azeezsalu" to the name you gave to your project)
unzip main.zip
cp -r techmax-main/* /var/www/html/
rm -rf techmax-main main.zip
systemctl enable httpd 
systemctl start httpd
