# AWS courses notes

- course: https://skillbuilder.aws/learn/94T2BEN85A/aws-cloud-practitioner-essentials/8D79F3AVR7

- Shared Responsibility Model
  - Overview

  - Security and Compliance is a shared responsibility between AWS and the customer. This shared model can help relieve the customer’s operational burden as AWS operates, manages and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates. The customer assumes responsibility and management of the guest operating system (including updates and security patches), other associated application software as well as the configuration of the AWS provided security group firewall. Customers should carefully consider the services they choose as their responsibilities vary depending on the services used, the integration of those services into their IT environment, and applicable laws and regulations. The nature of this shared responsibility also provides the flexibility and customer control that permits the deployment. As shown in the chart below, this differentiation of responsibility is commonly referred to as Security “of” the Cloud versus Security “in” the Cloud.

=============================================

# 1 Introductions to the cloud

- AWS 6 benefits
  - Key benefits of the AWS Cloud

- The six key benefits of the AWS Cloud are as follows.

- Trade fixed expense for variable expense
  - By using the AWS Cloud, businesses can transition from fixed investments to variable costs. With variable costs, customer expenses are better aligned with actual usage, thus creating more financial flexibility.

- Benefit from massive economies of scale
  - Like buying a product in bulk can result in lower prices per unit, the vast global infrastructure of AWS can result in lower costs for customers. This means that AWS can be used by many organizations, from small startups to major corporations. Businesses big and small can access advanced technologies that were previously only accessible to large enterprises.

- Stop guessing capacity
  - Customers can dynamically scale AWS Cloud resources up or down based on real-time demand. This means businesses can achieve optimal performance without provisioning more or less infrastructure than they need.

- Increase speed and agility
  - With the cloud, businesses can rapidly deploy applications and services, accelerating time to market and facilitating quicker responses to changing business needs and market conditions.

- Stop spending money to run and maintain data centers
  - The AWS Cloud eliminates the need for businesses to invest in physical data centers. This means customers aren't required to spend time and money on utilities and ongoing maintenance. With AWS taking care of the physical infrastructure of the cloud, customer resources can be reallocated to more strategic initiatives.

- Go global in minutes
  - Businesses don't need to set up their own infrastructure to expand internationally. AWS provides a robust global infrastructure that customers can use to deploy applications and services across multiple areas in minutes.

===================================

# 2 Compute in the cloud

- AWS region/az/datacenters
  - Region -> 3 or more Availability zones (AZs) -> 1 or more DataCenters
  - https://aws.amazon.com/about-aws/global-infrastructure/regions_az/

- Compute on AWS (overview)
  - This resource provides an overview of the different cloud computing services offered by AWS.

- AWS Compute Blog
  - This blog provides updates, tutorials, and best practices for using AWS compute services, such as Amazon EC2, AWS Lambda, Amazon ECS, and more.

- AWS Compute Services
  - This reference provides an in-depth introduction to the compute services available within the AWS Cloud.

- Hands-On Tutorials: Compute
  - This resource provides practical, step-by-step tutorials designed to help users gain hands-on experience with AWS compute services. It is ideal for beginners and those new to cloud computing.

- Amazon EC2
  - Amazon EC2 runs virtual servers in the cloud with flexible computing capacity.

- Amazon EC2 Instance Types
  - This guide provides detailed information about the different types of EC2 instances, including their specifications, capabilities, and use cases. It helps you choose the right instance type based on your workload needs, such as compute, memory, and storage requirements.

- Amazon EC2 Pricing
  - This guide explains the different pricing models for EC2 instances, including On-Demand, Reserved Instances, and Spot Instances, so you can choose the best option based on your usage.

- Amazon EC2 Auto Scaling
  - Amazon EC2 Auto Scaling automatically adjusts instance count based on demand for high availability and cost-efficiency.

- Elastic Load Balancing
  - Elastic Load Balancing automatically distributes incoming application traffic across multiple EC2 instances for high availability and fault tolerance.

- Amazon Simple Notification Service (SNS)
  - Amazon SNS is a messaging service for sending notifications to users or other applications through SMS, email, or mobile push notifications.

- Amazon Simple Queue Service (SQS)
  - Amazon SQS decouples application components through message queuing, storing and processing messages reliably.

============================

# 3 Exploring Compute services

- Services: managed (fully managed by AWS), unmanaged (you need to manage OS patching etc)
  - Key takeaways: Unmanaged and managed services

- AWS offers both unmanaged and managed services to suit different levels of control and responsibility. By understanding this model, you will know which tasks AWS manages and which you are responsible for, helping you secure and manage your cloud resources effectively.

- Unmanaged and managed services (details)
  - With unmanaged compute services like Amazon EC2, AWS takes care of the underlying physical infrastructure, but you're responsible for setting up, securing, and maintaining the operating system, network configurations, and applications on your instances. Managed services, on the other hand, reduce the amount of infrastructure you need to manage. While AWS handles much of the operational overhead, you might still need to perform some provisioning or configuration depending on the service. Using managed services shows a decrease in customer responsibility.

- Fully-managed services
  - Fully-managed services—like serverless ones—take abstraction even further, eliminating the need to provision or manage any servers at all. The underlying infrastructure is fully managed by AWS, so you can focus entirely on writing and deploying code. Later in this module, you will explore Lambda. Lambda is a serverless compute service where AWS handles the infrastructure, scaling, and availability, while you remain responsible for securing and managing your application code. Using full-managed services shows that the customer responsibility is even less than with managed services.

- Containers on AWS
  - The AWS Containers Services page provides an overview of the AWS container offerings, including services for container image storage, orchestration, and compute. These offerings are designed to streamline the deployment and management of containerized applications.

- Amazon Elastic Container Registry (ECR)
  - Amazon ECR is a fully managed service for storing, managing, and deploying container images securely at scale.

- Amazon Elastic Container Service (ECS)
  - Amazon ECS is a fully managed service that streamlines the deployment, management, and scaling of containerized applications on AWS.

- Amazon Elastic Kubernetes Service (EKS)
  - Amazon EKS is a fully managed Kubernetes service that streamlines running Kubernetes clusters on AWS and on premises. It automates infrastructure management and integrates with AWS networking, security, and storage services.

- AWS Fargate
  - Fargate is a serverless compute engine for running containers without managing servers. It is integrated with Amazon ECS and Amazon EKS.

- AWS Elastic Beanstalk
  - Elastic Beanstalk is a fully managed service for deploying and scaling web applications without managing infrastructure.

- AWS Batch
  - AWS Batch is a fully managed service for efficiently running large-scale batch computing jobs on AWS.

- What is Amazon Lightsail?
  - Lightsail is a simplified cloud platform offering VPS, containers, and databases with predictable pricing.

- What is AWS Outposts?
  - AWS Outposts extends AWS infrastructure and services to on-premises locations for low-latency, local data processing.

- Choosing a modern application strategy
  - The AWS Decision Guide for Modern Application Strategy helps organizations determine the most suitable development approach—serverless or Kubernetes—based on their operational model, team structure, and workload requirements.

====================

# 4 Introduction to Going Global

- Overview of foundational AWS Global Infrastructure
  - You've been introduced to some foundational elements of the AWS Global Infrastructure, such as AWS Regions and Availability Zones (AZs). In the following lessons, you will learn even more about AWS infrastructure. Concepts covered in these lessons include how to choose a Region, the value of edge locations, and how to use services such as AWS CloudFormation to streamline and automate deployment. In addition to achieving high availability, these components of the AWS Global Infrastructure can help your business achieve benefits like elasticity and agility.

- Going global with AWS infrastructure (coffee shop analogy)
  - The coffee shop is expanding to global locations. Navigate through the following content to review how elements of our coffee shop expansion represent different parts of the AWS Global Infrastructure.

- How to choose a Region or set of Regions
  - If we were to expand our coffee shop by opening new locations, there would be multiple things to consider, like customer demand and development cost. Similarly, you have several factors to consider when selecting a Region or set of Regions for your real-life resources.

- AWS edge locations
  - Like our coffee franchise could expand with smaller versions of the shop such as mobile coffee carts, AWS has smaller footprint facilities called edge locations. Edge locations cache items like images, videos, and other resources, so that users can access the content they need with lower latency. Edge locations, on the other hand, are part of the AWS content delivery network (CDN). They are optimized for content delivery, not directly tied to Availability Zones.

- Infrastructure as code and CloudFormation
  - Another important consideration of a coffee shop expansion would be to maintain a consistent product from location to location. AWS has services, such as CloudFormation, that you can use to help automate the deployment of your cloud resources. These services use infrastructure as code, or IaC, helping you achieve a consistent, reliable set up each time your business grows.

- Key considerations when choosing Regions: Compliance
  - Compliance is an important consideration when selecting Regions for deploying business resources. Different geographical locations have varying regulatory requirements and data protection laws that organizations must follow. For example, the General Data Protection Regulation (GDPR) is designed to protect the personal data and privacy of individuals within the European Union (EU). An online retail company operating in the EU would be required to meet GDPR compliance to protect customer data. GDPR compliance includes obtaining proper consent for data collection and providing mechanisms for data access and deletion.

- Proximity
  - When selecting a Region, you also want to consider how to achieve low latency for your users. Regions closer to your user base minimize data travel time, which reduces latency and enhances application responsiveness. Choosing a Region or set of Regions farther away from customers could introduce delays, which might impact user satisfaction and overall system efficiency.

- Feature availability
  - You also want to consider which specific features and services are available in each Region. AWS is constantly expanding features and services to multiple locations, but not all Regions contain all AWS offerings. For example, AWS GovCloud Regions are specifically designed to meet the compliance and security requirements of US government agencies and their contractors. These Regions have stringent physical, operational, and personnel security controls in place. These controls are only available in specific Regions to meet certain governmental regulatory requirements.

- Pricing
  - When selecting a Region, pricing is also a factor that can influence your decision. Some Regions have lower operational costs than others. These operational costs can impact the overall expenses for hosting applications and services. Tax laws and regulations can also play a role in cost. Some Regions might offer tax incentives or have lower tax rates, which can affect customer pricing. Additionally, data sovereignty laws in certain Regions might require data to be stored locally, affecting both compliance and cost.

- Edge locations (importance)
  - Edge locations are strategically placed sites around the world that cache content to deliver data, video, and applications with lower latency and higher transfer speeds. Edge locations are considered a vital part of the AWS content delivery network (CDN) and use services like CloudFront to efficiently distribute data to end users.

- Relationship between Regions, Availability Zones, and edge locations
  - Region (Regions are geographical areas around the world that are made up of multiple data center) -> 3 or more Availability zones (AZs) -> 1 or more DataCenters

- Regions description
  - Regions are geographical areas around the world that are made up of multiple data centers. These data centers provide scalable and redundant infrastructure for hosting cloud services. Each Region consists of multiple, isolated locations known as Availability Zones. Each Region has three or more Availability Zones.

- Availability Zones description
  - Availability Zones are distinct locations within a Region, each designed as an independent zone with its own power, networking, and connectivity. Availability Zones maintain high availability and fault tolerance for applications. Each Availability Zone consists of one or more data centers.

- Interacting with AWS resources
  - As you've learned, there are a number of ways you can operate in the AWS Cloud. To interact with AWS resources, you must invoke AWS APIs. To interact with these APIs, you can use the AWS SDKs, the AWS Command Line Interface (AWS CLI), the AWS Management Console, or IaC tools such as CloudFormation.

- CloudFormation (IaC)
  - CloudFormation is a service that helps you model and set up your AWS resources so that you can spend less time managing those resources and more time focusing on your applications that run in AWS. With CloudFormation, you can define your infrastructure as code. You create a template that describes all the AWS resources that you want (like Amazon Elastic Compute Cloud (Amazon EC2) instances), and CloudFormation takes care of provisioning and configuring those resources for you.

- Edge locations reminder
  - Edge locations are part of the AWS CDN and are optimized for content delivery, not directly tied to Availability Zones.

- Placement considerations summary
  - When deciding where to place cloud resources, companies must consider multiple factors. Compliance refers to the Region meeting legal or regulatory requirements. Proximity to customers helps reduce latency and improve user experience. Feature availability makes sure that the required AWS services are supported in the chosen Region. Pricing varies by Region, so cost-efficiency is also a critical factor.

==============================================

# 5 Introduction to Networking

- Describe what a virtual private cloud (VPC) is and what it does.
  - Describe what a subnet is and what it does.
  - Describe the difference between a public and private subnet.

- Networking overview
  - The term networking refers to interconnected devices that can exchange data and resources. Networking in the AWS Cloud consists of the infrastructure and services working together to host your applications, data, and any other resources you might need. Let's get started and learn about the foundational network components used in the AWS Cloud.

- Amazon Virtual Private Cloud (Amazon VPC)
  - An Amazon VPC lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define.

- Subnet
  - Subnets are used to organize your resources and can be made publicly or privately accessible. A private subnet is commonly used to contain resources like a database storing customer or transactional information. A public subnet is commonly used for resources like a customer-facing website.

- Define what a virtual private gateway is and what it does.
  - Identify the core components of a VPC.
  - Define an internet gateway and what it does.

- Amazon VPC (benefits)
  - With Amazon VPC, you can provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. It provides three main benefits. It helps increase security because you can secure and monitor connections, screen traffic, and restrict instance access. Amazon VPC gives you full control over your resource placement, connectivity, and security. The convenience of using Amazon VPC means you will spend less time setting up, managing, and validating your virtual network when compared to on-premises network management.

- Subnets (reiterated)
  - Within an Amazon VPC, you can organize your resources into subsections or subnets. A subnet is a section of an Amazon VPC that can contain resources, such as Amazon EC2 instances. You will learn more about subnets in the next lesson.

- Connecting your resources with an internet gateway
  - To allow public traffic from the internet to access your VPC, you attach an internet gateway to the VPC. An internet gateway is a connection between a VPC and the internet. You can think of an internet gateway as being similar to a doorway that customers use to enter the coffee shop. Without an internet gateway, no one can access the resources within your VPC.

- Virtual private gateways (VPN analogy)
  - What if you have a VPC that includes only private resources? The following example shows how a virtual private gateway works. You can think of the internet as the road between your home and the coffee shop. It is open and accessible to anyone. You want a way to protect the traffic you send on the internet from the public, internet service providers, and others who might be trying to track or intercept it. This is where a virtual private network (VPN) connection comes in.

- VPN (secure tunnel)
  - VPN creates a connection that is more like a secure tunnel through the internet. Using encryption, it hides and protects everything you send and receive from outside eyes. A virtual private gateway is the component in the AWS Cloud that makes it possible for you to connect this protected traffic to enter the VPC. With a VPN connection, your data travels privately and safely, hidden from others using the same route.

- Virtual private gateway (purpose)
  - With a virtual private gateway, you can establish a VPN connection between your VPC and a private network, such as an on-premises data center or internal corporate network. A virtual private gateway allows traffic into the VPC only if it is coming from an approved network.

- Amazon Virtual Private Cloud (summary)
  - Amazon VPC is used to establish boundaries around your AWS resources.

- Virtual private gateway (summary)
  - A virtual private gateway allows protected internet traffic to enter into the VPC.

- Virtual private network (VPN) (summary)
  - A VPN encrypts your internet traffic, helping protect it from anyone who might try to intercept or monitor it.

- Ways to connect to the AWS Cloud
  - With so many different types of networks, on-premises datacenters, and remote workers, companies need a wide range of ways to connect to the AWS Cloud. In the following section, you will learn four ways to connect to the AWS Cloud: AWS Client VPN, AWS Site-to-Site VPN, AWS PrivateLink, AWS Direct Connect.

- AWS Client VPN
  - AWS Client VPN is a networking service you can use to connect your remote workers and on-premises networks to the cloud. It is a fully managed, elastic VPN service that automatically scales up or down based on user demand. Because it is a cloud VPN solution, you don’t need to install and manage hardware or try to estimate how many remote users to support at one time.
  - Benefits: AWS Client VPN provides advanced authentication, remote access. It is elastic and fully managed.
  - Use case: It can be used to quickly scale remote-worker access.
  - Client VPN uses an OpenVPN-based client, and it works with global Regions by using the AWS global network.

- AWS Site-to-Site VPN
  - Site-to-Site VPN creates a secure connection between your data center or branch offices and your AWS Cloud resources.
  - Benefits: Site-to-Site VPN provides high availability, secure and private sessions, and accelerates applications.
  - Use cases: It can be used for application migration and secure communication between remote locations.

- AWS PrivateLink
  - AWS PrivateLink is a highly available, scalable technology that you can use to privately connect your VPC to services and resources as if they were in your VPC. You do not need to use an internet gateway, NAT device, public IP address, Direct Connect connection, or AWS Site-to-Site VPN connection to allow communication with AWS services or resources from your private subnets. Instead, you control the specific API endpoints, sites, services, and resources that are reachable from your VPC.
  - Benefits: AWS PrivateLink helps you secure your traffic and connect with simplified management rules.
  - Use case: It is used for connecting your clients in your VPC to resources, other VPCs, and endpoints.

- AWS Direct Connect
  - Direct Connect is a service that makes it possible for you to establish a dedicated private connection between your network and VPC in the AWS Cloud.
  - Benefits: AWS Direct Connect reduces network costs and increases amount of bandwidth.
  - Usage: A corporate data center routes network traffic to an AWS Direct Connect location. That traffic is then routed to a VPC through a virtual private gateway. All network traffic between the corporate data center and VPC flows through this dedicated private connection.

- Direct Connect use cases
  - latency sensitive apps: Direct Connect bypasses the internet and provides a consistent, low-latency network experience. This makes it ideal for applications like video streaming and other real-time applications that require high performance.
  - Large scale data migration or transfer: Direct Connect helps ensure smooth and reliable data transfers at massive scale for real-time analysis, rapid data backup, or broadcast media processing.
  - Hybrid cloud architecture: You can use Direct Connect to link your AWS and on-premises networks to build applications that span environments without compromising performance.

- Additional gateway services
  - AWS Transit Gateway is used to connect your Amazon VPCs and on-premises networks through a central hub. As your cloud infrastructure expands globally, inter-Region peering connects transit gateways together using the AWS Global Infrastructure.
  - NAT gateway: You can use a NAT gateway so that instances in a private subnet can connect to services outside your VPC but external services can't initiate a connection with those instances.
  - Amazon API Gateway: The Amazon API Gateway is an AWS service for creating, publishing, maintaining, monitoring, and securing APIs at any scale.

- VPC traffic and security controls
  - Describe how network traffic works in a VPC.
  - Describe how security groups work (stateful).
  - Describe how network access control lists (network ACLs) work (stateless).
  - Describe who is responsible for securing subnets with security groups and network ACLs according to the AWS Shared Responsibility Model.

- Hands-on steps
  - Navigate in the AWS Management Console.
  - Review the steps to create a VPC.
  - Create both public and private subnets.
  - Create and attach an internet gateway.
  - Create a route table, add routes, and associate public subnets.

- Demo summary
  - In the previous lessons, you have learned about the Amazon VPC and its core components. In this demonstration video, you will get to see the steps to bring it to reality. You will learn the steps to create a VPC, public and private subnets in two AZs, an internet gateway, and even routing tables.

- Global Networking: DNS, Route 53, CloudFront
  - Define what Domain Name System (DNS) is and what it does.
  - Describe benefits and use cases of Amazon Route 53.
  - Describe benefits and use cases of Amazon CloudFront.
  - DNS translates domain names/URLs entered by users to IP addresses that computers understand.

- Global Architectures (VPN, Direct Connect, CloudFront, Route 53)
  - Identify examples of when to use a VPN or Direct Connect.
  - Describe at a high level how a VPC with a virtual private network (VPN) connection and Direct Connect work together.
  - Describe how a multi-Region architecture works with CloudFront and Route 53.
  - Summary: networking involves VPC, subnets, gateway, routing table, Amazon Route 53 DNS; for global network: Route 53 -> CloudFront -> closest edge location -> VPC in Region.

- VPN vs Direct Connect summary
  - VPN for privacy/security of data; Direct Connect for privacy/security and large data.
  - Combination of VPN and Direct Connect, or multiple Direct Connects for fail-safe network.

- CloudFront
  - CloudFront speeds up distribution of your static and dynamic web content to your users. It securely delivers your content with low latency through a worldwide network of data centers called edge locations.

- ACLs and Security Groups
  - ACLs for subnet, Security groups for EC2 instances.

- Core networking components (recap)
  - Amazon Virtual Private Cloud (VPC)
  - Subnet
  - Internet gateway
  - Virtual private gateway
  - AWS Client VPN
  - AWS Site-to-Site VPN
  - AWS PrivateLink
  - AWS Direct Connect
  - Network Access Control List (network ACL)
  - Security groups
  - Domain Name System (DNS)
  - Amazon Route 53
  - Amazon CloudFront
  - AWS Global Accelerator
  - Amazon Transit Gateway
  - NAT Gateway
  - API Gateway

=================================

# 6 Introduction to Storage

- Storage types summary
  - 3 types of storage are supported by AWS: Block storage, Object storage, File storage.

- Block storage (overview)
  - Block storage is like accessing your hard drive, basically volumes attached to EC2 instances.

- EC2 instance store
  - Amazon EC2 instance store (temporary volume, erased when EC2 instance is deleted), high performance.

- Amazon EBS (Elastic Block Store)
  - Amazon EBS provides persistent block-level storage volumes for use with Amazon EC2 instances. EBS volumes act like external hard drives, offering consistent and low-latency performance for workloads like databases and file systems. EBS volumes can be conveniently backed up, resized, and attached to different EC2 instances. To create an EBS volume, you define the configuration for things like volume size and type. After the volume has been created, it can be attached to an Amazon EC2 instance. Because EBS volumes are for data that needs to persist, it’s important to back up the data. It's recommended that you take incremental backups of EBS volumes by creating Amazon EBS snapshots.

- Object Storage
  - Object Storage: like COS bucket in IBM Cloud, AWS S3.

- File storage
  - File storage: Linux NFS or file shares across a network.

- Amazon FSx
  - FSx: Windows and other file systems, SMB. Non-NFS, non-Linux.

- Links and references
  - https://aws.amazon.com/ebs/faqs/
  - https://aws.amazon.com/s3/faqs/
  - https://aws.amazon.com/efs/faq/

- EC2 Instance Store User Guide
  - A temporary storage option that is directly attached to the host computer of an EC2 instance, providing high-performance but non-persistent storage.

- Amazon EBS (links)
  - Amazon Elastic Block Store (Amazon EBS) — a scalable block storage service that provides persistent, high-performance volumes you can attach to your EC2 instances for data storage and applications.
  - Amazon Elastic Block Store (Amazon EBS) FAQ — https://aws.amazon.com/ebs/faqs/
  - Amazon EBS Snapshots User Guide — EBS Snapshots are point-in-time backups of your cloud storage volumes, making it possible to protect data and restore it when needed.
  - Amazon Data Lifecycle Manager User Guide — a service that streamlines the creation, retention, and deletion of Amazon EBS snapshots.

- Amazon S3 (links)
  - Amazon Simple Storage Service (Amazon S3) — a scalable cloud storage service that can store and retrieve any amount of data from anywhere on the web.
  - Amazon S3 FAQ — https://aws.amazon.com/s3/faqs/
  - Amazon S3 Storage Classes — various storage classes tailored to different access and cost needs.
  - Amazon S3 Versioning User Guide — keeps multiple variants of objects for recovery.
  - Amazon S3 Buckets User Guide — S3 buckets are cloud storage containers.

- Amazon EFS
  - Amazon Elastic File System (Amazon EFS) — a scalable, fully-managed file storage service that lets multiple AWS resources access shared data simultaneously without capacity planning.
  - Amazon EFS FAQ — https://aws.amazon.com/efs/faq/

- Amazon FSx options
  - Amazon FSx — fully managed file storage service with options including Windows File Server, NetApp ONTAP, OpenZFS, and Lustre.
  - FSx for Windows File Server — provides reliable, high-performance file storage compatible with Windows applications.
  - FSx for NetApp ONTAP — provides advanced data management capabilities for Windows and Linux workloads.
  - FSx for OpenZFS — high-performance, scalable storage using ZFS.
  - FSx for Lustre — designed to accelerate compute-intensive workloads.

- AWS Storage Gateway and configurations
  - AWS Storage Gateway — hybrid cloud storage service that integrates on-premises environments with AWS cloud storage services.
  - Amazon S3 File Gateway — provides local file access to S3 objects while caching frequently accessed data locally.
  - Tape Gateway — used for backing up data to Amazon S3 while maintaining compatibility with tape-based backup applications.
  - Volume Gateway — provides iSCSI block storage volumes to on-premises applications, offering cached and stored modes.

===============================

# 7 Databases

- Amazon RDS
  - Amazon Relational Database Service (Amazon RDS) — a relational database service supporting multiple engines like MySQL, PostgreSQL, and Microsoft SQL Server with automated maintenance and backups.

- Amazon RDS Security and Aurora
  - Amazon RDS Security — detailed information about security configurations in Amazon RDS.
  - Amazon Aurora — a cloud-native database offering superior performance and availability over traditional databases while maintaining MySQL and PostgreSQL compatibility.

- AWS Database Migration Service (DMS)
  - A service that provides seamless database migration between source and target databases while keeping the source database operational.

- Amazon DynamoDB
  - A NoSQL database service providing single-digit millisecond performance at any scale with built-in security.

- Amazon ElastiCache
  - An in-memory caching service that supports Redis, Valkey, or Memcached to improve application performance through faster data retrieval.

- Amazon DocumentDB
  - A MongoDB-compatible document database service designed for mission-critical workloads with automatic scaling.

- Amazon Backup
  - A centralized service for automating and managing data backups across AWS services and on-premises resources.

- Amazon Neptune
  - A graph database service optimized for storing and querying highly connected data relationships (like graph data in social media).

- What Is a Relational Database?
  - A structured database using tables with predefined schemas, supporting complex queries and transactions through SQL for consistent data relationships.

- What Is a NoSQL Database?
  - A nonrelational database offering flexible schemas and high scalability for varied data types, optimized for specific data models and patterns.

- What Is an In-Memory Caching Service?
  - A high-speed data storage layer using RAM instead of disk storage, delivering microsecond latency for frequently accessed data.

- AWS Shared Responsibility Model (reminder)
  - AWS is responsible for security of the cloud (infrastructure, hardware, networking, facilities) while customers are responsible for security in the cloud (data, configuration, access management).

===============================================

# 8 AI/ML/Data Analytics

- Amazon Comprehend
  - Use natural language processing to extract key insights from documents.

- Amazon Polly
  - Convert text into lifelike speech.

- Amazon Transcribe
  - Convert speech into text.

- Amazon Translate
  - Translate text into multiple languages.

- Amazon Kendra
  - Use natural language processing to intelligently query enterprise content.

- Amazon Rekognition
  - Identify objects and activities in images and videos.

- Amazon Textract
  - Detect and extract typed and handwritten text in documents.

- Amazon Lex
  - Add voice and text conversational interfaces to applications.

- Amazon Personalize
  - Add personalized customer recommendations to applications.

- Amazon SageMaker
  - Build, train, and deploy your own ML models without worrying about infrastructure.

- Amazon SageMaker JumpStart
  - Deploy pre-trained ML solutions, like computer vision, NLP, and tabular data, with just a few clicks.

- Amazon Bedrock
  - Fine-tune and seamlessly integrate large foundation models from Amazon and leading AI startups into your AWS applications with a single API.

- Amazon Q Business and Developer
  - Amazon Q Business — Answer questions and solve problems using the data and expertise found in your company's information repositories.
  - Amazon Q Developer — Accelerate development with code recommendations.

- Streaming and ingestion
  - Amazon Kinesis Data Streams — Ingest terabytes of streaming data in real time.
  - Amazon Data Firehose — Ingest and deliver data within seconds to multiple consumers, such as data lakes and warehouses.

- Storage and analytics services
  - Amazon S3 — Store virtually limitless amounts of all types of data using this popular data lake choice.
  - Amazon Redshift — Store petabytes of structured or semistructured data in this data warehouse service. Analyze large datasets stored in the warehouse using complex SQL queries.
  - AWS Glue Data Catalog — Provide metadata to various analytics services with this centralized repository.
  - AWS Glue — Process data by using the AWS Glue Data Catalog as a reference.
  - Amazon EMR — Process big data workloads by using popular frameworks like Apache Spark.
  - Amazon Athena — Analyze various data sources hosted anywhere with a single SQL query.
  - Amazon QuickSight — Visualize data by creating interactive dashboards with or without expertise.
  - Amazon OpenSearch Service — Visualize and monitor real-time data analytics with keyword or NLP searches.

=====================================================

# 9 Security

- Authentication vs authorization
  - Basic distinction between proving identity (authentication) and granting rights (authorization).

- IAM concepts
  - IAM, IAM users, IAM Group, IAM policy, IAM roles.
  - Principle of least privilege, grant roles for temporary access.

- AWS Identity and Access Management (IAM)
  - Securely manage identities and access to AWS services and resources.

- AWS IAM Identity Center
  - Connect your existing workforce identity source and centrally manage access to AWS with single sign-on.

- AWS Secrets Manager
  - Centrally store and manage credentials, API keys, and other secrets.

- AWS Systems Manager
  - Manage nodes, or connection points, at scale on AWS and in multi-cloud and hybrid environments.

- AWS Shield
  - Protect your network and applications from the most common, frequently occurring types of DDoS attacks.

- AWS WAF
  - Protect your network and applications from blocked IP addresses defined by a web ACL.

- AWS Key Management Service (KMS)
  - Create and manage cryptographic keys to encrypt and decrypt your data.

- Amazon Macie
  - Discover and protect sensitive data in Amazon S3.

- AWS Certificate Manager (ACM)
  - Create and manage SSL/TLS certificates that provide data encryption in transit.

- Amazon Inspector
  - Check applications for security vulnerabilities and deviations from security best practices.

- Amazon GuardDuty
  - Continuously monitor the AWS environment with intelligent threat detection.

- Amazon Detective
  - Analyze threats with interactive visualizations contained in a unified view.

- AWS Security Hub
  - Aggregate security findings and organize them into actionable insights.

=======================================

# 10 Monitoring, Compliance, and Governance in AWS Cloud

- Module summary
  - In this module, you learned the progression of securing, monitoring, auditing, compliance, and governance in the AWS Cloud. You identified services that aid in monitoring with metrics, alarms, and dashboards. You also learned about services for auditing, such as CloudTrail, and compliance, such as AWS Artifact. You reviewed several other governance and compliance services and identified the role of AWS Trusted Advisor in continuously evaluating for cost, security, performance, and more.

- Amazon CloudWatch
  - CloudWatch monitors your AWS resources and the applications you run on AWS in real time. With CloudWatch, you gain system-wide visibility into resource utilization, application performance, and operational health.

- AWS CloudTrail
  - CloudTrail enables auditing, security monitoring, and operational troubleshooting. CloudTrail records user activity and API calls across AWS services as events. CloudTrail events help you answer the question of "Who did what, where, and when?"

- AWS Artifact
  - AWS Artifact is a self-service portal that provides on-demand access to AWS security and compliance documentation, including reports, certifications, and agreements.

- AWS Config
  - AWS Config is a service to assess, audit, and evaluate the configurations of your AWS resources.

- AWS Audit Manager
  - Audit Manager is a service to continually audit your AWS usage to streamline risk and compliance assessment.

- AWS Organizations
  - Organizations helps you centrally manage and govern your environment as you grow and scale your AWS resources. It helps you manage policies for groups of accounts and automate account creation.

- AWS Control Tower
  - With AWS Control Tower, you can enforce and manage governance rules for security, operations, and compliance at scale across all your organizations and accounts in the AWS Cloud.

- AWS Service Catalog
  - With Service Catalog, you can create, share, and organize from a curated catalog of AWS resources. You can deploy baseline networking resources and security tools for new AWS accounts so you can govern consistently.

- AWS License Manager
  - License Manager is a service that helps you manage your software licenses and fine-tune your licensing costs.

- AWS Trusted Advisor
  - Trusted Advisor helps you optimize costs, increase performance, improve security and resilience, and operate at scale in the cloud. It continuously evaluates your AWS environment using best practice checks across those categories and recommends actions to remediate deviations from best practices.

- AWS Health
  - AWS Health is the data source for events and changes affecting your AWS Cloud resources. AWS Health notifies you about service events, planned changes, and account notifications to help you manage and take actions.

- IAM Access Analyzer
  - IAM Access Analyzer provides capabilities to set, verify, and refine security permissions to achieve least privilege security standards.

========================================================================

# 11 Pricing and Support

- Module summary
  - In the last few lessons, you learned about AWS pricing concepts and AWS support options. You covered fundamental pricing concepts and services. You also learned the difference between AWS Support Plans and other technical assistance resources. Finally, you applied these concepts to a real-world application by thinking about how to optimize for cost in the AWS Cloud. Next in your AWS Cloud Practitioner learning journey, you will consider the basic principles, strategies, and services for migrating resources to the cloud.

- Amazon S3 Pricing
  - The Amazon S3 Pricing page outlines costs for storage, requests, data transfer, and additional features, along with details on AWS Free Tier for new customers.

- Amazon EC2 On-Demand Pricing
  - The Amazon EC2 On-Demand Pricing page details the costs for EC2 instances, including pricing for instance types, data transfer, and additional features with no long-term commitments.

- What is AWS Organizations?
  - The AWS Organizations User Guide explains how to centrally manage multiple AWS accounts, automate account creation, apply governance policies, and simplify billing and resource sharing.

- AWS Billing Console
  - The AWS Billing Console provides a centralized platform for managing and understanding AWS charges, offering tools to view and download invoices, monitor discounts and credits, and analyze spending trends across multiple accounts.

- AWS Budgets
  - AWS Budgets provides tools to create custom budgets for tracking and managing AWS costs, usage, and Reserved Instance or Savings Plan use. It also helps prevent overspending by offering alerts and automated actions.

- AWS Cost Explorer
  - AWS Cost Explorer provides tools to visualize, analyze, and manage AWS costs and usage, with customizable reports and cost forecasting to optimize cloud spending.

- AWS Pricing Calculator Documentation
  - The AWS Pricing Calculator is a free, web-based tool that helps customers create detailed cost estimates for AWS services, so they can plan and manage their cloud expenditures effectively.

- AWS re:Post
  - AWS re:Post is a community-driven, question-and-answer platform provided where users can seek help, share knowledge, and find solutions related to AWS services and technologies.

- AWS Trust and Safety Center
  - The AWS Trust and Safety Center offers guidance on reporting abuse, protecting applications, and following best practices for digital messaging on AWS.

- AWS Professional Services
  - The AWS Professional Services page highlights how AWS experts help organizations accelerate cloud adoption with tailored guidance across industries and technologies.

- AWS Documentation
  - The AWS Documentation page provides comprehensive technical resources, including guides, API references, tutorials, and best practices across AWS services.

- AWS Marketplace
  - The AWS Marketplace is a digital catalog where customers can discover, purchase, and manage third-party software, data, and services with flexible pricing options.

- Engage with AWS Partners and Partner resources
  - Engage with AWS Partners, funding benefits, partner events, training and certification opportunities.

==================================================================================

# 12 Migrating to the AWS Cloud

- Recap and next steps
  - In this migration module, you identified the AWS Cloud Adoption Framework (AWS CAF), the seven migration strategies, and migration services to migrate applications, databases, and data.

- Three Phases of Migration
  - In performing a large-scale migration, there are typically three phases: assess, mobilize, and the last phase, migrate and modernize.

- AWS Cloud Adoption Framework (AWS CAF)
  - AWS CAF is a framework that brings AWS experience and best practices to companies preparing to migrate to the AWS Cloud. The framework provides tools to help accelerate the migration journey, organize resources, and align management during the transition.

- Seven Migration Strategies (7 Rs)
  - When migrating to the cloud, there are seven common migration strategies that customers can choose to implement. They are relocate, rehost, replatform, refactor, repurchase, retain, and retire.

- Migration Evaluator
  - The Migration Evaluator is a migration assessment service that helps you create a business case for AWS Cloud planning and migration. It does this with a data-driven approach, analyzing your current state and target state, and developing a migration readiness plan with projected cloud costs.

- AWS Application Discovery Service
  - Application Discovery Service discovers on-premises server inventory and connections. It gathers configuration, performance, and connection details for both servers and databases to create a detailed migration plan.

- AWS Application Migration Service
  - Application Migration Service is a tool to migrate and improve your on-premises and cloud-based applications. It helps customers simplify, expedite, and reduce the cost of migrating and modernizing applications.

- AWS Migration Hub
  - Migration Hub is a centralized hub to take you from discovery to assessment, planning, and implementation of your migration. It provides tools, guidance, and automated recommendations to collaborate with your team and track your migration.

- AWS Database Migration Service (DMS)
  - AWS DMS makes it possible to quickly and securely migrate databases to the AWS Cloud. It provides a way to plan, assess, convert, and migrate databases even with data warehouses in one central tool.

- AWS Schema Conversion Tool (SCT)
  - AWS SCT is a service that makes it possible to convert database schemas and code objects (like stored procedures, views, and functions) from one database engine to another.

- AWS DataSync
  - DataSync is specifically designed for automating and accelerating secure data migrations. DataSync manages data movement workloads with bandwidth throttling, migration scheduling, task filtering, and task reporting. It also provides rapid data replication.

- AWS Transfer Family
  - Transfer Family makes it possible to seamlessly manage and share data with simple, secure, and scalable file transfers. This service provides fully managed support for secure file transfers over SFTP, FTPS, FTP, and others. It helps you transfer files directly into and out of AWS storage services like Amazon S3 and Amazon EFS.

- AWS Direct Connect (recap)
  - Direct Connect is a cloud service that you can use to establish a private, dedicated network connection between your on-premises network and AWS.

- AWS Snow Family
  - AWS Snowball Edge Storage Optimized devices are a great solution for offline data migration where connecting to the internet might not be an option. Snowball Edge Storage Optimized devices deliver high performance storage, and make it possible to simplify multi-petabyte data migrations from on-premises locations to AWS.

==============================================================================
