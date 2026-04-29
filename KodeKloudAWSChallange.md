# Day 1: Create Key Pair
  # Requirement:
        The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the AWS cloud. Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps rather than as a single massive transition. To achieve this, they have segmented large tasks into smaller, more manageable units. This granular approach enables the team to execute the migration in gradual phases, ensuring smoother implementation and minimizing disruption to ongoing operations. By breaking down the migration into smaller tasks, the Nautilus DevOps team can systematically progress through each stage, allowing for better control, risk mitigation, and optimization of resources throughout the migration process.

        For this task, create a key pair with the following requirements:

        Name of the key pair should be datacenter-kp.

        Key pair type must be rsa

        Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

        Console URL	https://093501631776.signin.aws.amazon.com/console?region=us-east-1
        Username	kk_labs_user_411033
        Password	24Q5z9GLT%dl
        Start Time	Sat Mar 14 18:26:30 UTC 2026
        End Time	Sat Mar 14 19:26:30 UTC 2026

        Notes:

        Create the resources only in us-east-1 region.

        To display or hide the terminal of the AWS client machine, you can use the expand toggle button as shown below:
        toggle button

  # Solution:
        Navigate to Keypairs option in Conslole
            KeyPairs --> Create Key Pair --> Enter name --> select rsa as Keypairtype --> Click on create keypair

# Day 2: Create Security Group
  # Requirement:
      The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the AWS cloud. Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps rather than as a single massive transition. To achieve this, they have segmented large tasks into smaller, more manageable units. This granular approach enables the team to execute the migration in gradual phases, ensuring smoother implementation and minimizing disruption to ongoing operations. By breaking down the migration into smaller tasks, the Nautilus DevOps team can systematically progress through each stage, allowing for better control, risk mitigation, and optimization of resources throughout the migration process.

            For this task, create a security group under default VPC with the following requirements:

            Name of the security group is datacenter-sg.

            The description must be Security group for Nautilus App Servers

            Add the inbound rule of type HTTP, with port range of 80. Enter the source CIDR range of 0.0.0.0/0.

            Add another inbound rule of type SSH, with port range of 22. Enter the source CIDR range of 0.0.0.0/0.



            Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

            Console URL	https://351481091276.signin.aws.amazon.com/console?region=us-east-1
            Username	kk_labs_user_645701
            Password	Q!VIJB!Q6TuN
            Start Time	Sun Mar 15 20:46:54 UTC 2026
            End Time	Sun Mar 15 21:46:54 UTC 2026

  # Solution:
            Navigate to VPC form search
            Navigate to Default VPC --> Navigate to Security groups --> Click create security group --> Provide the mentioned details in requirement --> click on create

# Day 4: Enable Versioning for S3 Bucket
  # Requirement:
      Data protection and recovery are fundamental aspects of data management. It's essential to have systems in place to ensure that data can be recovered in case of accidental deletion or corruption. The DevOps team has received a requirement for implementing such measures for one of the S3 buckets they are managing.

            The s3 bucket name is devops-s3-28498, enable versioning for this bucket.

            Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

            Console URL	https://392284424672.signin.aws.amazon.com/console?region=us-east-1
            Username	kk_labs_user_681355
            Password	UZBtnwDB@7sq
            Start Time	Tue Mar 24 17:05:47 UTC 2026
            End Time	Tue Mar 24 18:05:47 UTC 2026

            Notes:

            Create the resources only in us-east-1 region.
            To display or hide the terminal of the AWS client machine, you can use the expand toggle button as shown below:\n

   # Solution:
      Navigate to S3 --> Open the Bucket --> navigate to Properties --> Bucket Versioning --> Enable --> Save
      More info about S3 -->
      https://github.com/sampath-devops/aws-devops-zero-to-hero/blob/main/day-9/README.md

# Day 5: Create GP3 Volume
  # Requirement:
    
     The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the AWS cloud. Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps rather than as a single massive transition. To achieve this, they have segmented large tasks into smaller, more manageable units. This granular approach enables the team to execute the migration in gradual phases, ensuring smoother implementation and minimizing disruption to ongoing operations. By breaking down the migration into smaller tasks, the Nautilus DevOps team can systematically progress through each stage, allowing for better control, risk mitigation, and optimization of resources throughout the migration process.

      Create a volume with the following requirements:

      Name of the volume should be xfusion-volume.

      Volume type must be gp3.

      Volume size must be 2 GiB.



      Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

      Console URL	https://163665808200.signin.aws.amazon.com/console?region=us-east-1
      Username	kk_labs_user_914954
      Password	zBFYbgWy54jP
      Start Time	Mon Apr 06 11:03:57 UTC 2026
      End Time	Mon Apr 06 12:03:57 UTC 2026

      Notes:

      Create the resources only in us-east-1 region.

      To display or hide the terminal of the AWS client machine, you can use the expand toggle button as shown below:
      toggle button
   # Solution:

      1. Navigate to Volumes: In the Amazon EC2 Console, choose Volumes under the Elastic Block Store section in the left navigation pane.
      2. Create Volume: Click the Create volume button.
          Configure Settings:
          Volume type: Select General Purpose SSD (gp3).
          Size: Enter the desired size in GiB - 2GIB


# Day 6: Launch EC2 Instance
   # Requirement:
      The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the AWS cloud. Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps rather than as a single massive transition. To achieve this, they have segmented large tasks into smaller, more manageable units.

        For this task, create an EC2 instance with following requirements:

        1) The name of the instance must be datacenter-ec2.

        2) You can use the Amazon Linux AMI to launch this instance.

        3) The Instance type must be t2.micro.

        4) Create a new RSA key pair named datacenter-kp.

        5) Attach the default (available by default) security group.



        Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

        Console URL	https://658733160186.signin.aws.amazon.com/console?region=us-east-1
        Username	kk_labs_user_112689
        Password	fZi@%JC4NWz!
        Start Time	Tue Apr 07 11:52:54 UTC 2026
        End Time	Tue Apr 07 12:52:54 UTC 2026




        Notes:

        Create the instance in us-east-1 region.

        To display or hide the terminal of the AWS client machine, you can use the expand toggle button as shown below:
        toggle button

   # Solution:  
      Name and Tags: Give your instance a name (e.g., "datacenter-ec2") to help identify it later.
      Choose an OS (AMI): Select an Amazon Machine Image (AMI), which is the template for your operating system (e.g., Amazon Linux, Ubuntu, or Windows).
      Select Instance Type: Choose a hardware configuration based on your CPU and RAM needs.
      Tip: For testing, the t2.micro or t3.micro types are often Free Tier eligible. 
      Security and Access
      Key Pair: Select an existing key pair or Create a new key pair to securely connect via SSH (Linux) or RDP (Windows).

# Day 7: Change EC2 Instance Type
  # Requirement:
      During the migration process, the Nautilus DevOps team created several EC2 instances in different regions. They are currently in the process of identifying the correct resources and utilization and are making continuous changes to ensure optimal resource utilization. Recently, they discovered that one of the EC2 instances was underutilized, prompting them to decide to change the instance type. Please make sure the Status check is completed (if its still in Initializing state) before making any changes to the instance.

        1) Change the instance type from t2.micro to t2.nano for datacenter-ec2 instance.

        2) Make sure the ec2 instance datacenter-ec2 is in running state after the change.



        Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

        Console URL	https://933196964255.signin.aws.amazon.com/console?region=us-east-1
        Username	kk_labs_user_612791
        Password	28^tghFR%0R2
        Start Time	Thu Apr 16 10:12:58 UTC 2026
        End Time	Thu Apr 16 11:12:58 UTC 2026
  # Solution: 

      1. Navigate to the datacenter-ec2 instance
      2. Stop the instance as we can not change the instance type when it is running
      3. Once instance stopped navigate to the Instance state options click on change the instance type and change the state to t2.nano
      4. Start the instance once instance is changed

# Day 8: Enable Stop Protection for EC2 Instance
  # Requirement:
      As part of the migration, there were some components added to the AWS account. Team created one of the EC2 instances where they need to make some changes now.

        There is an EC2 instance named datacenter-ec2 under us-east-1 region, enable the stop protection for this instance.



        Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

        Console URL	https://538701479232.signin.aws.amazon.com/console?region=us-east-1
        Username	kk_labs_user_450745
        Password	Xt^WlW@Q0nGB
        Start Time	Tue Apr 21 04:28:37 UTC 2026
        End Time	Tue Apr 21 05:28:37 UTC 2026

  # Solution:
      1. Navigate to the EC2 instance 
      2. Go to Actions --> Instance Settings --> Click on Change stop protection --> Click on Enable --> Save the changes
      3. we can see the change stop protection setting will be changed to enable from disable state in instance details
      4. Enabling stop protection on an EC2 instance prevents accidental shutdowns, ensuring high availability for stateful    workloads and preventing data loss           from ephemeral storage. It acts as a safety mechanism against unintentional stop or termination commands via the console, CLI, or API, enforcing a two-            step process to shut down critical production/staging servers. 
       
        Key Benefits of EC2 Stop Protection:
            Prevent Accidental Downtime: Protects critical servers from accidental manual or scripted shutdowns.
            Data Protection: Safeguards data in ephemeral instance store volumes that would otherwise be lost if the instance is stopped or terminated.
            Support for Stateful Workloads: Ideal for applications that cannot handle sudden interruptions, ensuring they stay running until specifically intended             otherwise.
            Operational Security: Adds a required step of disabling the protection first, reducing "fat-finger" errors, as highlighted in this LinkedIn post. 
            Usage Examples & Synonyms:
            Usage Examples: Protecting production database instances, ensuring high-availability database servers (e.g., MySQL, PostgreSQL) on EC2 do not go down              during maintenance windows.
            Synonyms/Related Concepts: Instance stop prevention, unintended action safeguard, safety latch, resource safety belt.

# Day 9: Enable Termination Protection for EC2 Instance
  # Requirement:  
      As part of the migration, there were some components created under the AWS account. The Nautilus DevOps team created one EC2 instance where they forgot to enable the termination protection which is needed for this instance.

      An instance named nautilus-ec2 already exists in us-east-1 region. Enable termination protection for the same.



      Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

      Console URL	https://621551581842.signin.aws.amazon.com/console?region=us-east-1
      Username	kk_labs_user_895278
      Password	2r6C^J6scaav
      Start Time	Wed Apr 22 16:42:55 UTC 2026
      End Time	Wed Apr 22 17:42:55 UTC 2026
  # Solution:
      1. Navigate to the EC2 instance 
      2. Go to Actions --> Instance Settings --> Click on Change termination protection --> Click on Enable --> Save the changes
      3. we can see the change termination protection setting will be changed to enable from disable state in instance details

      Amazon EC2 termination protection is a safety feature that prevents accidental deletion of instances via the console, CLI, or API, acting as a safeguard for critical infrastructure. It ensures that instances cannot be terminated until the attribute is explicitly disabled, protecting against data loss and unintended service disruptions. 

        Key Benefits of EC2 Termination Protection:
        Prevents Accidental Termination: It provides a critical safety mechanism, preventing accidental clicks in the AWS Management Console or misguided scripts from terminating production instances.
        Data Preservation: By stopping unintentional termination, it secures the data stored on attached Elastic Block Store (EBS) volumes, which are otherwise permanently deleted when an instance is terminated.
        Reduces Unplanned Downtime: It enhances high availability by adding an extra step to the shutdown process, preventing service outages caused by human error or improper automation.
        Secure Production Workloads: This is a vital practice for protecting important servers, separating production systems from non-critical or test environments.
        Configurable Security: Termination protection can be enabled upon launch, or on running/stopped instances, offering flexible security settings

# Day 10: Attach Elastic IP to EC2 Instance
  # Requirement:
    The Nautilus DevOps team has been creating a couple of services on AWS cloud. They have been breaking down the migration into smaller tasks, allowing for better control, risk mitigation, and optimization of resources throughout the migration process. Recently they came up with requirements mentioned below.

      There is an instance named nautilus-ec2 and an elastic-ip named nautilus-ec2-eip in us-east-1 region. Attach the nautilus-ec2-eip elastic-ip to the nautilus-ec2 instance.



      Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

      Console URL	https://471339402762.signin.aws.amazon.com/console?region=us-east-1
      Username	kk_labs_user_928314
      Password	KVd0cYp^ukIi
      Start Time	Thu Apr 23 07:20:18 UTC 2026
      End Time	Thu Apr 23 08:20:18 UTC 2026

  # Solution:

      Assigning an Elastic IP to an Amazon EC2 instance involves two primary phases: allocating a static IP address to your AWS account and then associating it with your specific instance. 
     
      Phase 1: Allocate a New Elastic IP 
      Before you can attach an IP, you must reserve one from the AWS pool. 
    
      Sign in to the AWS Management Console.
      In the left navigation pane of the Amazon EC2 Console, scroll down to Network & Security and select Elastic IPs.
      Click the Allocate Elastic IP address button.
      Choose Amazon's pool of IPv4 addresses (unless you are bringing your own IP range).
      Click Allocate. You will see the new IP address listed in your dashboard. 
    
      Phase 2: Associate the IP with an EC2 Instance 
      Once allocated, you must link the IP to your running instance. 
      
      In the Elastic IPs dashboard, select the checkbox next to the IP address you just created.
      Click the Actions dropdown menu and select Associate Elastic IP address.
      For Resource type, ensure Instance is selected.
      In the Instance field, select your EC2 instance from the list.
      (Optional) Select the specific Private IP address to associate with if your instance has multiple.
      Click Associate. 

# Day 11: Attach Elastic Network Interface to EC2 Instance
  # Requirement:
      The Nautilus DevOps team has been creating a couple of services on AWS cloud. They have been breaking down the migration into smaller tasks, allowing for better control, risk mitigation, and optimization of resources throughout the migration process. Recently they came up with requirements mentioned below.

        An instance named nautilus-ec2 and an elastic network interface named nautilus-eni already exists in us-east-1 region.

        Attach the nautilus-eni network interface to the nautilus-ec2 instance.
        Make sure status is attached before submitting the task.
        Please make sure instance initialisation has been completed before submitting this task.



        Use below given AWS Credentials. (You can run the showcreds command on aws-client host to retrieve these credentials)

        Console URL	https://240365323441.signin.aws.amazon.com/console?region=us-east-1
        Username	kk_labs_user_317994
        Password	cwlXu98kgj@a
        Start Time	Fri Apr 24 17:26:06 UTC 2026
        End Time	Fri Apr 24 18:26:06 UTC 2026
  # Solution:
    1. Validate both Instance and Network interfaces are available or not
    2. Navigate to Network interface --> Click on attach --> Select the VPC --> Select the Ec2 instance
    3. Click on attach 

# Day 12: Attach Volume to EC2 Instance
  # Requirement:
      The Nautilus DevOps team has been creating a couple of services on AWS cloud. They have been breaking down the migration into smaller tasks, allowing for better control, risk mitigation, and optimization of resources throughout the migration process. Recently they came up with requirements mentioned below.

        An instance named devops-ec2 and a volume named devops-volume already exists in us-east-1 region. Attach the devops-volume volume to the devops-ec2 instance, make sure to set the device name to /dev/sdb while attaching the volume.



        Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

        Console URL	https://223308557377.signin.aws.amazon.com/console?region=us-east-1
        Username	kk_labs_user_902690
        Password	l7tMz!Weg%Z0
        Start Time	Sat Apr 25 18:06:46 UTC 2026
        End Time	Sat Apr 25 19:06:46 UTC 2026

  # Solution:
      1. Navigate to the Volumes --> Select the Volume named Devops-volume --> Go to Actions --> Select attach --> Select the Ec2 instance --> select the device name as specified --> Attach -- This will attach the volume to Ec2 instance and we can review it in EC2 instance under storage section


# Day 13: Create AMI from EC2 Instance
  # Requirement:
    The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the AWS cloud. Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps rather than as a single massive transition. To achieve this, they have segmented large tasks into smaller, more manageable units. This granular approach enables the team to execute the migration in gradual phases, ensuring smoother implementation and minimizing disruption to ongoing operations. By breaking down the migration into smaller tasks, the Nautilus DevOps team can systematically progress through each stage, allowing for better control, risk mitigation, and optimization of resources throughout the migration process.

      For this task, create an AMI from an existing EC2 instance named xfusion-ec2 with the following requirement:

      Name of the AMI should be xfusion-ec2-ami, make sure AMI is in available state.



      Use below given AWS Credentials: (You can run the showcreds command on aws-client host to retrieve these credentials)

      Console URL	https://278810891986.signin.aws.amazon.com/console?region=us-east-1
      Username	kk_labs_user_239659
      Password	1^uelvEgEOSP
      Start Time	Wed Apr 29 04:45:06 UTC 2026
      End Time	Wed Apr 29 05:45:06 UTC 2026
  # Solution:

      Creating an Amazon Machine Image (AMI) from an existing EC2 instance can be done through the AWS Management Console, the Command Line Interface (CLI), or specific developer tools. 
      Method 1: Using the AWS Management Console
                This is the most common method for manual image creation. 
                Stop the Instance (Recommended): While you can create an AMI from a running instance, it is highly recommended to stop it first to ensure data consistency across all volumes.
                Select Instance: Log in to the AWS Management Console, navigate to EC2 > Instances, and select the instance you want to use.
                Choose Create Image: Click the Actions button, then select Image and templates > Create image.
                Configure Image:
                Image name: Provide a unique name for your AMI.
                Description: (Optional) Add details about the software or configuration included.
                No reboot: By default, AWS reboots the instance during this process to ensure a clean state. Check "No reboot" only if you must keep the instance running, though this risks file system integrity.
                Create Image: Click Create image at the bottom of the page.
                Monitor Progress: Go to the AMIs section in the left navigation pane. The status will stay "pending" for several minutes until it becomes "available". 
    
      Method 2: Using the AWS CLI
              You can create an AMI using the AWS CLI create-image command. 
            
              Basic Command:
              bash
              aws ec2 create-image --instance-id i-1234567890abcdef0 --name "MyServerImage" --description "AMI for web server"
              Without Reboot: To skip the default reboot, add the --no-reboot flag:
              bash
              aws ec2 create-image --instance-id i-1234567890abcdef0 --name "MyServerImage" --no-reboot
      
      Method 3: Using Other Tools
            AWS Toolkit for Visual Studio: Right-click an instance in the AWS Toolkit Explorer and select Create Image (EBS AMI).
            AWS Tools for PowerShell: Use the New-EC2Image cmdlet to perform the same action from a Windows environment. 
      
      Important Considerations
                Root Volume: The resulting AMI will include a snapshot of the root EBS volume and any other EBS volumes attached to the instance.
                Billing: While creating an AMI is free, you will be charged for the EBS snapshot storage used by the image.
                Region: AMIs are region-specific. If you need to use the image in a different region, you must first copy the AMI to that region. 
  
