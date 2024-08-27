# EC2-Instance-with-an-Elastic-IP-on-AWS
Setting Up an EC2 Instance with an Elastic IP for Application Hosting
To set up an EC2 instance named `datacenter-ec2` and associate an Elastic IP named `datacenter-eip`, you can follow these steps using the AWS Management Console:

### 1. **Log in to the AWS Management Console**
   - Open your browser and navigate to the [AWS Management Console](https://767398003596.signin.aws.amazon.com/console?region=us-east-1).
   - Log in using the provided credentials: 
     - Username: `kk_labs_user_614559`
     - Password: `M4J8ykuABmRh`

### 2. **Launch a New EC2 Instance**
   - Go to the **EC2 Dashboard** by selecting "EC2" from the AWS services menu.
   - Click on **Launch Instance**.
   - Name your instance `xfusion-ec2`.
   - **Choose an AMI**: Select an Ubuntu AMI or any other Linux-based AMI.
   - **Instance Type**: Choose `t2.micro` (eligible for the free tier).
   - **Key Pair (login)**: Select an existing key pair or create a new one if required.
   - **Network Settings**: 
     - Choose the default VPC and subnet.
     - Make sure to allow SSH (port 22) access in the security group to log in.
   - Click **Launch Instance**.

### 3. **Allocate an Elastic IP**
   - Go to the **Elastic IPs** section in the EC2 Dashboard.
   - Click **Allocate Elastic IP address**.
   - Click **Allocate** to create a new Elastic IP.
   - Once created, click on the new Elastic IP and click **Actions** -> **Associate Elastic IP address**.

### 4. **Associate the Elastic IP with the EC2 Instance**
   - In the **Associate Elastic IP** screen:
     - Select your EC2 instance `datacenter-ec2`.
     - Click **Associate**.
   - Your instance should now be associated with the Elastic IP.

### 5. **Name the Elastic IP**
   - In the **Elastic IPs** section, select the newly created Elastic IP.
   - Click on the pencil icon next to the name and rename it to `xfusion-eip`.

### 6. **Verify the Setup**
   - In the EC2 Dashboard, check that the `datacenter-ec2` instance is running and has the Elastic IP `datacenter-eip` associated with it.

### 7. **Log Out**
   - Once everything is set up and verified, log out of the AWS Console.

By following these steps, you'll have successfully created an EC2 instance with a stable IP address, fulfilling the Development Team's requirements.
