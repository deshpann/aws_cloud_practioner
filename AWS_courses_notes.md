# AWS courses notes:

- course: https://skillbuilder.aws/learn/94T2BEN85A/aws-cloud-practitioner-essentials/8D79F3AVR7

- Shared Responsibility Model — Overview

  Security and Compliance is a shared responsibility between AWS and the customer. This shared model can help relieve the customer’s operational burden as AWS operates, manages and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates. The customer assumes responsibility and management of the guest operating system (including updates and security patches), other associated application software as well as the configuration of the AWS provided security group firewall. Customers should carefully consider the services they choose as their responsibilities vary depending on the services used, the integration of those services into their IT environment, and applicable laws and regulations. The nature of this shared responsibility also provides the flexibility and customer control that permits the deployment. As shown in the chart below, this differentiation of responsibility is commonly referred to as Security “of” the Cloud versus Security “in” the Cloud.

=============================================

# 1 Introductions to the cloud

- AWS 6 benefits — Key benefits of the AWS Cloud

- Trade fixed expense for variable expense

  By using the AWS Cloud, businesses can transition from fixed investments to variable costs. With variable costs, customer expenses are better aligned with actual usage, thus creating more financial flexibility.

- Benefit from massive economies of scale

  Like buying a product in bulk can result in lower prices per unit, the vast global infrastructure of AWS can result in lower costs for customers. This means that AWS can be used by many organizations, from small startups to major corporations. Businesses big and small can access advanced technologies that were previously only accessible to large enterprises.

- Stop guessing capacity

  Customers can dynamically scale AWS Cloud resources up or down based on real-time demand. This means businesses can achieve optimal performance without provisioning more or less infrastructure than they need.

- Increase speed and agility

  With the cloud, businesses can rapidly deploy applications and services, accelerating time to market and facilitating quicker responses to changing business needs and market conditions.

- Stop spending money to run and maintain data centers

  The AWS Cloud eliminates the need for businesses to invest in physical data centers. This means customers aren't required to spend time and money on utilities and ongoing maintenance. With AWS taking care of the physical infrastructure of the cloud, customer resources can be reallocated to more strategic initiatives.

- Go global in minutes

  Businesses don't need to set up their own infrastructure to expand internationally. AWS provides a robust global infrastructure that customers can use to deploy applications and services across multiple areas in minutes.

===================================

# 2 Compute in the cloud

- AWS region/az/datacenters — Region -> 3 or more Availability Zones (AZs) -> 1 or more DataCenters

  https://aws.amazon.com/about-aws/global-infrastructure/regions_az/

- Compute on AWS (overview resources and docs)

  This resource provides an overview of the different cloud computing services offered by AWS.

- AWS Compute Blog, Compute Services, Hands-On Tutorials

  Blog provides updates, tutorials, and best practices for using AWS compute services, such as Amazon EC2, AWS Lambda, Amazon ECS, and more. The reference provides an in-depth introduction to compute services. Hands-on tutorials help users gain practical experience.

- Amazon EC2

  Amazon EC2 runs virtual servers in the cloud with flexible computing capacity.

- Amazon EC2 Instance Types

  Guide describing different EC2 instance types and use cases.

- Amazon EC2 Pricing

  Pricing models for EC2: On-Demand, Reserved Instances, Spot Instances.

- Amazon EC2 Auto Scaling & Elastic Load Balancing

  Auto Scaling adjusts instance counts based on demand; Elastic Load Balancing distributes incoming application traffic across EC2 instances.

- Amazon SNS and Amazon SQS

  SNS is a messaging/notification service. SQS decouples components through message queuing.

============================

# 3 Exploring Compute services

- Services: managed (fully managed by AWS), unmanaged (you need to manage OS patching etc)

  Key takeaways: Unmanaged and managed services — understand which tasks AWS manages and which the customer is responsible for.

- Unmanaged and managed services (explanation)

  With unmanaged compute services like Amazon EC2, AWS takes care of the underlying physical infrastructure, but you're responsible for OS, network configs, and applications. Managed services reduce the operational overhead; fully-managed serverless services (e.g., Lambda) eliminate server provisioning and management.

- Containers on AWS, ECR, ECS, EKS, Fargate, Elastic Beanstalk, Batch

  Overview of AWS container offerings and related services: Amazon ECR (container registry), ECS (orchestration), EKS (managed Kubernetes), Fargate (serverless containers), Elastic Beanstalk (managed app deployment), AWS Batch (batch jobs).

- Other compute offerings: Lightsail, Outposts

  Lightsail: simplified VPS and predictable pricing. Outposts: extends AWS infra to on-premises for low-latency local processing.

- Choosing a modern application strategy

  The AWS Decision Guide helps determine whether to use serverless or Kubernetes based on operational model and workload needs.

====================

# 4 Introduction to Going Global

- Overview: regions, AZs, choosing regions, edge locations, CloudFormation

  Learn how to choose a Region, value of edge locations, and use services such as CloudFormation for automation. These help achieve high availability, elasticity, and agility.

- Going global with AWS infrastructure (coffee shop analogy)

  The coffee shop expansion maps to AWS global infrastructure elements (regions, AZs, edge locations).

- How to choose a Region or set of Regions

  Consider customer demand, development cost, compliance, latency, feature availability, and pricing.

- AWS edge locations

  Edge locations cache content (images, videos) to reduce latency; part of the CDN (CloudFront) and optimized for content delivery, not tied to AZs.

- Infrastructure as Code and CloudFormation

  CloudFormation automates and standardizes deployments using templates to define desired AWS resources.

- Key considerations when choosing Regions: Compliance, Proximity, Feature availability, Pricing

  Compliance (e.g., GDPR), proximity for low latency, check features available in a region, and consider pricing and tax/regulatory impacts.

- Edge locations (again) and relationship between Regions, AZs, and edge locations

  Edge locations cache and deliver content; Regions are geographic areas made up of multiple AZs; AZs are isolated locations with one or more data centers.

- Interacting with AWS resources

  Use AWS SDKs, CLI, Management Console, or IaC tools like CloudFormation to invoke AWS APIs.

- CloudFormation (summary)

  Define templates describing AWS resources and let CloudFormation provision and configure them.

==============================================

# 5 Introduction to Networking

- Networking fundamentals: VPC, subnet, public vs private subnet

  Networking in AWS consists of infrastructure and services to host applications and data. A VPC is a logically isolated virtual network; subnets organize resources and can be public or private.

- Amazon Virtual Private Cloud (VPC) — definition

  VPC lets you provision an isolated section of the AWS Cloud where you launch AWS resources in a virtual network you define.

- Subnet — definition

  Subnets are sections of a VPC that contain resources such as EC2 instances.

- Internet gateway — definition and purpose

  To allow public internet traffic to access a VPC, attach an Internet Gateway to the VPC. It is the connection between a VPC and the internet.

- Virtual private gateway, VPN, and secure connections

  VPN creates a secure tunnel over the internet. A virtual private gateway enables VPN connections into the VPC, allowing approved networks to communicate securely.

- Summary of VPC, virtual private gateway, VPN

  VPC establishes boundaries; virtual private gateway allows protected traffic into the VPC; VPN encrypts internet traffic.

- Ways to connect to AWS Cloud: Client VPN, Site-to-Site VPN, PrivateLink, Direct Connect

  Client VPN (fully managed) for remote workers; Site-to-Site VPN for secure connections with on-prem data centers; PrivateLink for private connectivity to services/endpoints; Direct Connect for dedicated private connections and higher bandwidth.

- AWS Client VPN details

  Fully managed elastic VPN using OpenVPN-based clients for remote access and advanced authentication.

- AWS Site-to-Site VPN details

  Creates secure connections between data centers/branch offices and AWS resources; useful for migrations and secure communications.

- AWS PrivateLink details

  Privately connect your VPC to services without internet gateway, NAT, public IPs, Direct Connect, or Site-to-Site VPN.

- AWS Direct Connect details

  Dedicated private connection between your network and AWS for lower latency, consistent performance, and large data transfers. Use cases include latency-sensitive apps, large-scale data migration, and hybrid cloud architectures.

- Additional gateway services: Transit Gateway, NAT Gateway, API Gateway

  Transit Gateway connects VPCs and on-prem through a hub. NAT Gateway allows private subnet instances outbound internet access. API Gateway manages APIs at scale.

- VPC traffic, security groups (stateful), network ACLs (stateless), and shared responsibility

  Network traffic flows in VPCs are controlled by security groups (stateful, instance-level) and network ACLs (stateless, subnet-level). Customers are responsible for configuring these according to the AWS Shared Responsibility Model.

- Hands-on: creating a VPC, subnets, IGW, route table, and associating public subnets

  Steps include creating VPC, public/private subnets across AZs, attaching an internet gateway, and configuring routes and associations.

- Global Networking, DNS, Route 53, and CloudFront

  DNS translates domain names to IP addresses. Route 53 is AWS DNS and routing service. CloudFront is the CDN that accelerates content delivery via edge locations.

- Global Architectures: VPN vs Direct Connect, multi-Region with CloudFront and Route 53

  VPN provides security; Direct Connect provides dedicated private connectivity for large data and performance; both can be combined for resilience.

- Summary: networking components and flow

  Key networking components: VPC, subnets, gateways, routing tables, Route 53, CloudFront, edge locations; ACLs protect subnets, security groups protect instances.

=================================

# 6 Introduction to Storage

- Storage types in AWS: Block, Object, File

  AWS supports block storage (volumes attached to EC2), object storage (S3), and file storage (EFS, FSx).

- Block storage: EC2 instance store and EBS

  Instance store: temporary, erased when the instance stops/terminates. EBS: persistent block-level volumes for EC2 with snapshot backup and lifecycle management.

- EBS features & backups

  EBS volumes act like external hard drives; recommended incremental backups via EBS snapshots; Data Lifecycle Manager can automate snapshot lifecycles.

- Object storage: Amazon S3

  S3 stores and retrieves any amount of data; offers storage classes, versioning, and bucket management.

- File storage: Amazon EFS and Amazon FSx

  EFS provides scalable, shared file storage for Linux. FSx provides managed file systems for Windows, Lustre, NetApp ONTAP, OpenZFS.

- AWS Storage Gateway and its configurations

  Storage Gateway provides hybrid cloud integration: S3 File Gateway (local file access to S3), Tape Gateway (backup compatibility), Volume Gateway (iSCSI block storage for on-prem apps).

- Links and documentation references (EBS, S3, EFS FAQs and guides)

  https://aws.amazon.com/ebs/faqs/ ; https://aws.amazon.com/s3/faqs/ ; https://aws.amazon.com/efs/faq/

===============================

# 7 Databases

- Amazon RDS

  Managed relational database service supporting MySQL, PostgreSQL, SQL Server with automated maintenance and backups.

- Amazon RDS Security and Aurora

  RDS security best practices. Amazon Aurora is a cloud-native database offering high performance while remaining MySQL/Postgres compatible.

- AWS Database Migration Service (DMS)

  Seamless database migration service that keeps the source DB operational during migration.

- Amazon DynamoDB

  NoSQL database with single-digit millisecond performance at any scale.

- Amazon ElastiCache

  In-memory caching (Redis, Memcached) to improve application performance.

- Amazon DocumentDB

  MongoDB-compatible document database service for mission-critical workloads.

- Amazon Backup

  Centralized service for automating backups across AWS and on-prem resources.

- Amazon Neptune

  Graph database service optimized for highly connected data (e.g., social graphs).

- What is relational vs NoSQL vs in-memory cache

  Relational DBs use structured schemas and SQL; NoSQL offers flexible schemas and high scale; in-memory caches use RAM for microsecond latency for frequently accessed data.

- AWS Shared Responsibility Model (reminder)

  AWS secures the cloud infrastructure; customers secure data, configuration, and access in the cloud.

===============================================

# 8 AI/ML/Data Analytics

- AWS AI/ML services overview: Comprehend, Polly, Transcribe, Translate, Kendra, Rekognition, Textract, Lex

  Services for NLP, speech-to-text, text-to-speech, translation, intelligent search, image/video analysis, document text extraction, and conversational interfaces.

- Personalize, SageMaker, JumpStart, Bedrock, Amazon Q

  Personalize adds recommendations; SageMaker builds, trains, and deploys ML models; JumpStart offers pre-trained solutions; Bedrock integrates large foundation models; Amazon Q provides question-answering for business data and developer acceleration tools.

- Streaming and ingestion: Kinesis Data Streams, Data Firehose

  Services for ingesting and delivering streaming data to data lakes and analytics.

- Storage and analytics: S3, Redshift, Glue, EMR, Athena, QuickSight, OpenSearch

  S3 as data lake; Redshift for petabyte-scale data warehousing; Glue for ETL and data catalog; EMR for big data frameworks; Athena for SQL querying; QuickSight for dashboards; OpenSearch for search and monitoring.

=====================================================

# 9 Security

- IAM and access controls

  AWS Identity and Access Management (IAM) securely manages identities and access to services and resources.

- IAM Identity Center and Secrets Manager

  IAM Identity Center centralizes SSO and workforce identity. Secrets Manager stores credentials and API keys securely.

- Systems Manager for node management

  AWS Systems Manager helps manage nodes at scale across AWS and hybrid environments.

- Threat protection: Shield, WAF, Inspector, GuardDuty, Detective

  Shield protects against DDoS. WAF protects apps from common web exploits. Inspector checks for vulnerabilities. GuardDuty provides continuous threat detection. Detective analyzes threats visually.

- Key management and data protection: KMS, ACM, Macie

  KMS creates and manages cryptographic keys. ACM manages SSL/TLS certificates. Macie discovers and protects sensitive data in S3.

- Security Hub

  Aggregates security findings into actionable insights.

- Summary: security tooling and responsibilities

  AWS provides broad security tooling; customers must use these and configure access, encryption, and monitoring according to the Shared Responsibility Model.