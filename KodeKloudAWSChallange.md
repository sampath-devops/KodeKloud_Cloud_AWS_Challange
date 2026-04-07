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

