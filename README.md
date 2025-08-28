# Deploying-managing-services-in-AWS

TASKs
A)
1. Create a private RDS instance using a sandbox template.
2. The engine type must be MySQL v8.4.5, and it must be a db.t3.micro type instance.
3. the master username should be changed with an appropriate password.
4. The RDS storage type must be gp2, and the storage size must be 5GiB.
5. Create a database .
6. Keep the rest of the configurations as default. Ensure the instance is in available state.
7. Adjust the security groups so that the ec2 instance can connect to the RDS on port 3306 and also open port 80 for the instance.

B)
2) An EC2 instance exists. Connect to this instance from the AWS console. Create an SSH key (/root/.ssh/id_rsa) on the aws-client host if it doesn't already exist. Add the public key to the authorized keys of the root user on the EC2 instance for password-less SSH access.

C)
3) There is a file named index.php under the /root directory on the aws-client host. Copy this file to the ec2 instance under the /var/www/html/ directory. Make the appropriate changes in the file to connect to the RDS.
D)
4) You should see a Connected successfully message in the browser once you access the instance using the public IP.

