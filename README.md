# EC2-Instance-for-a-webpage-AWS
This is laboratory for creating an EC2 instance for a website
# Set Up an EC2 Instance
Sign in to the Management console of your AWS account and go to the EC2 dashboard, click on "Launch Instance![create instance](https://github.com/user-attachments/assets/d93e0e70-486a-42b0-ba92-9b33fe8cc0d0)
Give the instance a name & choose amazon machine image![Give instance a name](https://github.com/user-attachments/assets/cb7f937d-e4a6-48c6-b4da-573dd4cbe031)
Select an instance type and create a key pair for SSH access![Instance Type](https://github.com/user-attachments/assets/5b884859-29c2-44bc-a750-b4631edec7eb)
Configure security group rules and allow SSH and HTTP or HTTPS traffic![Configure Security](https://github.com/user-attachments/assets/7996fcc0-4647-4884-86e3-d7e5b887d432)
Click "launch Instance then you will be able to view new and old instances.![Launch Instance](https://github.com/user-attachments/assets/b5b6fdad-31ba-4dcb-bd9d-aa630094fd77)
Use an SSH client to connect to the instance using public Ip, the key pair and Username and click on connect. ![Connect to Instance](https://github.com/user-attachments/assets/02309241-3e31-497e-bffe-2888350f361b)
# Install and Configure a Web Server
Switch to root user (sudo -i) and Update the Instance(sudo yum update -y). ![Switch User](https://github.com/user-attachments/assets/41132470-dfd2-492d-a8ec-49d62a43a586)
Install Apache Web Server(sudo yum install httpd -y). ![Apache Web server](https://github.com/user-attachments/assets/70bd3e91-b6cf-4035-afba-ad873b83e6f5)
Start the Apache Web server service(sudo systemctl start httpd).![Apache Web server](https://github.com/user-attachments/assets/edade0de-81e4-48b3-8dfc-ba8b0951501d)
Check if the apache web server is enabled and also confirm the status(sudo systemctl enable httpd) & (sudo systemctl status httpd).![Enable apache](https://github.com/user-attachments/assets/1dbc1cda-e2ce-4078-89e0-70914a4fc3e2)
Set up  temp directory(mkdir temp) and change to the "temp" directory.![Temp directory](https://github.com/user-attachments/assets/eb33033d-bc28-45fa-a811-3d41e80a2805)
Use wget command and copy the download free css template directly to your web server instance.![Using wget command to download the free template](https://github.com/user-attachments/assets/e80ffa17-6ee9-43c1-8fb8-1b1ae76782b4)
Unzip the downloaded file with unzip command(unzip oxer.zip).![Unzip dowloaded file](https://github.com/user-attachments/assets/f5de9043-7c7c-4993-9f76-d78e2eefbbfd)
Change directory to the oxer.html file and move content of the /var/www/html.![changing directory to the oxer html file and move content of file](https://github.com/user-attachments/assets/c644de9b-c702-450e-9201-90117796b2da)
# Access the Website
Open your web browser and navigate to the public IP address of the EC2 instance.![Access your Website](https://github.com/user-attachments/assets/65143554-f641-4bf8-89e9-ac9f9f9b503e)
