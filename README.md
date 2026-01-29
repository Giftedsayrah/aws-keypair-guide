# aws-keypair-guide

This guide demonstrates how to create an RSA key pair in AWS using the Management Console (GUI). Key pairs are used to securely connect to EC2 instances via SSH.
Region used: us-east-1
Key pair name: nautilus-kp
Key type: RSA

*Step 1: Log in to AWS Console*
1.	Open your browser and go to the AWS Console URL:
https://625000249352.signin.aws.amazon.com/console?region=us-east-1
2.	Enter your credentials: for example  
-Username: labs_user_575004
-Password: BatfQbRHO8
4.	Ensure the region in the top-right corner is set to US East (N. Virginia) – us-east-1.


*Step 2: Navigate to EC2 Dashboard*
1.	In the Services menu, search for EC2.
2.	Click EC2 to open the EC2 Dashboard.


*Step 3: Open Key Pairs Section*
1.	On the left-hand menu, scroll down to Network & Security.
2.	Click Key Pairs.


*Step 4: Create a New Key Pair*
1.	Click the Create key pair button.
2.	Fill in the details:
o	Key pair name: nautilus-kp
o	Key pair type: RSA
o	Private key file format: .pem (default for SSH)
3.	Click Create key pair.
   

*Step 5: Download the Private Key*
•	After creation, the .pem file will automatically download.
•	Important: Save this file securely. This is your only copy of the private key.


*Step 6: Verify the Key Pair*
1.	In the Key Pairs section, you should see nautilus-kp listed.
2.	Click it to view Key pair details, including Key type (RSA) and Fingerprint.

   

Best Practices

•	Keep the .pem file secure; without it, SSH access to EC2 instances will fail.

•	For phased cloud migration, consider creating separate key pairs for development, staging, and production environments.

