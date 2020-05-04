<h2>EC2 SERVICE IN AWS<h2>
  
<h3>What is Amazon EC2?<h3>


<p>Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) cloud. Using Amazon EC2 eliminates your need to invest in hardware up front, so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. Amazon EC2 enables you to scale up or down to handle changes in requirements or spikes in popularity, reducing your need to forecast traffic.</p> 


<h3>Features of Amazon EC2<h3>

Amazon EC2 provides the following features:
	* Virtual computing environments, known as instances
	* Various configurations of CPU, memory, storage, and networking capacity for your instances, known as instance types
	* Secure login information for your instances using key pairs (AWS stores the public key, and you store the private                  		key in a secure place) 
	* Storage volumes for temporary data that's deleted when you stop or terminate your instance, known as instance store 		volumes
	* Multiple physical locations for your resources, such as instances and Amazon EBS volumes, known as Regions and 	   Availability Zones
	* A firewall that enables you to specify the protocols, ports, and source IP ranges that can reach your instances 		using security groups
	* Static IPv4 addresses for dynamic cloud computing, known as Elastic IP addresses
	* Metadata, known as tags, that you can create and assign to your Amazon EC2 resources 
	* Virtual networks you can create that are logically isolated from the rest of the AWS cloud, and that you can 		  optionally connect to your own network, known as virtual private clouds (VPCs)
	
	
How to start and use EC2 service ?
	steps:
	1. create aws account 
	2. create New Ec2 instance for either in Amazon linux os/Linux os/Windows os
	3. create Key pair It is used to log in to your instance securely.  
	4. Create a security group for making rules of like inbound rules and outbound rules.

<h2>Best practices for Amazon EC2<h2>
	This list of practices will help you get the maximum benefit from Amazon EC2. 
	**Security**
	    * Manage access to AWS resources and APIs using identity federation, IAM users, and IAM roles. Establish 		      credential management policies and procedures for creating, distributing, rotating, and revoking AWS access 	        credentials. For more information, see IAM Best Practices in the IAM User Guide.
	    * Implement the least permissive rules for your security group. For more information, see Security Group Rules.
	    * Regularly patch, update, and secure the operating system and applications on your instance. For more 		      information about updating Amazon Linux 2 or the Amazon Linux AMI, see Managing Software on Your Linux Instance   	      in the Amazon EC2 User Guide for Linux Instances.
	
	**Storage**
	    * Understand the implications of the root device type for data persistence, backup, and recovery. For more 		      information, see Storage for the root device.

    	    * Use separate Amazon EBS volumes for the operating system versus your data. Ensure that the volume with your 		data persists after instance termination. For more information, see Preserving Amazon EBS Volumes on Instance 		    Termination.

    	    * Use the instance store available for your instance to store temporary data. Remember that the data stored in 		 instance store is deleted when you stop or terminate your instance. If you use instance store for database 		      storage, ensure that you have a cluster with a replication factor that ensures fault tolerance.

	    * Encrypt EBS volumes and snapshots. For more information, see Amazon EBS encryption.


	**Resource management**

    	    * Use instance metadata and custom resource tags to track and identify your AWS resources. For more information, 		   see Instance metadata and user data and Tagging your Amazon EC2 resources.

   	    * View your current limits for Amazon EC2. Plan to request any limit increases in advance of the time that you'll 		    need them. For more information, see Amazon EC2 Service Quotas.
	    
	**Backup and recovery**

   	    * Regularly back up your EBS volumes using Amazon EBS snapshots, and create an Amazon Machine Image (AMI) from 		 your instance to save the configuration as a template for launching future instances.

    	    * Deploy critical components of your application across multiple Availability Zones, and replicate your data   		 appropriately.

    	    * Design your applications to handle dynamic IP addressing when your instance restarts. For more information, see 		    Amazon EC2 Instance IP Addressing.

    	    * Monitor and respond to events. For more information, see Monitoring Amazon EC2.

   	    * Ensure that you are prepared to handle failover. For a basic solution, you can manually attach a network 		      interface or Elastic IP address to a replacement instance. For more information, see Elastic Network 		      Interfaces. For an automated solution, you can use Amazon EC2 Auto Scaling. For more information, see the 	      Amazon EC2 Auto Scaling User Guide.

   	    * Regularly test the process of recovering your instances and Amazon EBS volumes if they fail.





	
