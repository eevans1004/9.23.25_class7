Creating a basic EC2 server instance from a custom github script:
Navigate and log in to your AWS Management Console as IAM user.
Click "EC2"
Click "Launch instance"
Name your instance in "Name and tags" field
Scroll down the page to "Key pair (login)" field - 
Click "proceed without a key pair"
Scroll down to "Network settings" -"Firewall (security groups)
Click 'edit"
Select an existing security group
Click "Advanced details"
Scroll down to "User data" field
Copy the script and paste the EC2 startup script code from Theo's bmc5 repository into User data field
Click "Launch instance"
Click the instance number (begins with i-xxxxxx) after the instance spins up
Copy the Public DNS number
Open a new browser window and paste the following into the URL field (http://"public DNS number")
Click Enter and the EC2 instance should begin
To teardown instance:
Navigate to "Instances" tab
Select your running instance
Click "Instance state"
Select "Terminate (delete) instance"
