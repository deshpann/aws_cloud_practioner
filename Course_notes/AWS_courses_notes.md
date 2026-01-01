# AWS courses notes (formatted)

---

## AWS 6 benefits

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

---

## AWS region/az/datacenters -Region->3 or more Availability zones(AZs)-> 1 or more DataCenters

- https://aws.amazon.com/about-aws/global-infrastructure/regions_az/

---

## Services:

- managed(fully managed by aws), unmanaged(you need to manage os patching etc) 
Key takeaways: Unmanaged and managed services

- AWS offers both unmanaged and managed services to suit different levels of control and responsibility. By understanding this model, you will know which tasks AWS manages and which you are responsible for, helping you secure and manage your cloud resources effectively.

- Unmanaged and managed services

- With unmanaged compute services like Amazon EC2, AWS takes care of the underlying physical infrastructure, but you're responsible for setting up, securing, and maintaining the operating system, network configurations, and applications on your instances. Managed services, on the other hand, reduce the amount of infrastructure you need to manage. While AWS handles much of the operational overhead, you might still need to perform some provisioning or configuration depending on the service.

- Using managed services shows a decrease in customer responsibility.

- Fully-managed services

- Fully-managed services—like serverless ones—take abstraction even further, eliminating the need to provision or manage any servers at all. The underlying infrastructure is fully managed by AWS, so you can focus entirely on writing and deploying code. Later in this module, you will explore Lambda. Lambda is a serverless compute service where AWS handles the infrastructure, scaling, and availability, while you remain responsible for securing and managing your application code.

- Using full-managed services shows that the customer responsibility is even less than with managed services.

- Services and details:

- Amazon EC2(opens in a new tab)
Amazon EC2 runs virtual servers in the cloud with flexible computing capacity.

- Amazon EC2 Instance Types(opens in a new tab)
This guide provides detailed information about the different types of EC2 instances, including their specifications, capabilities, and use cases. It helps you choose the right instance type based on your workload needs, such as compute, memory, and storage requirements.

- Amazon EC2 Pricing(opens in a new tab)
This guide explains the different pricing models for EC2 instances, including On-Demand, Reserved Instances, and Spot Instances, so you can choose the best option based on your usage.

- Amazon EC2 Auto Scaling(opens in a new tab)
Amazon EC2 Auto Scaling automatically adjusts instance count based on demand for high availability and cost-efficiency.

- Elastic Load Balancing(opens in a new tab)
Elastic Load Balancing automatically distributes incoming application traffic across multiple EC2 instances for high availability and fault tolerance.

- Amazon Simple Notification Service(opens in a new tab)
Amazon SNS is a messaging service for sending notifications to users or other applications through SMS, email, or mobile push notifications.

- Amazon Simple Queue Service(opens in a new tab)
Amazon SQS decouples application components through message queuing, storing and processing messages reliably.

- Lamda: serverless, event driven
Lambda use cases
Lambda is ideal for building responsive, event-driven applications across a wide range of industries. Here are three real-world examples that show how Lambda helps companies scale efficiently, reduce operational overhead, and only pay for what they use.

- container services: ecs, eks, ecr(registry)

- container hosting platforms: ec2(you manage infra) or fargate(fully managed by aws) 

- Extra services to help: https://render.skillbuilder.aws/?module_id=D18S53TDBA%3A001.000.000&product_id=8D79F3AVR7%3A002.000.000&registration_id=fe7a03a2-36cb-5ecf-8a98-f0f580cc34b5&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital

- Containers on AWS(opens in a new tab)
The AWS Containers Services page provides an overview of the AWS container offerings, including services for container image storage, orchestration, and compute. These offerings are designed to streamline the deployment and management of containerized applications.

- Amazon Elastic Container Registry(opens in a new tab)
The Amazon ECR is a fully managed service for storing, managing, and deploying container images securely at scale.

- Amazon Elastic Container Service(opens in a new tab)
Amazon ECS is a fully managed service that streamlines the deployment, management, and scaling of containerized applications on AWS.

- Amazon Elastic Kubernetes Service(opens in a new tab)
Amazon EKS is a fully managed Kubernetes service that streamlines running Kubernetes clusters on AWS and on premises. It automates infrastructure management and integrates with AWS networking, security, and storage services.

- AWS Fargate(opens in a new tab)
Fargate is a serverless compute engine for running containers without managing servers. It is integrated with Amazon ECS and Amazon EKS.

- AWS Elastic Beanstalk(opens in a new tab)
Elastic Beanstalk is a fully managed service for deploying and scaling web applications without managing infrastructure.

- AWS Batch(opens in a new tab)
AWS Batch is a fully managed service for efficiently running large-scale batch computing jobs on AWS.

- What is Amazon Lightsail?(opens in a new tab)
Lightsail is a simplified cloud platform offering VPS, containers, and databases with predictable pricing.

- What is AWS Outposts?(opens in a new tab)
AWS Outposts extends AWS infrastructure and services to on-premises locations for low-latency, local data processing.

- Choosing a modern application strategy(opens in a new tab)
The AWS Decision Guide for Modern Application Strategy helps organizations determine the most suitable development approach—serverless or Kubernetes—based on their operational model, team structure, and workload requirements.

---

## Introduction to Going Global

- You've been introduced to some foundational elements of the AWS Global Infrastructure, such as AWS Regions and Availability Zones (AZs). In the following lessons, you will learn even more about AWS infrastructure. Concepts covered in these lessons include how to choose a Region, the value of edge locations, and how to use services such as AWS CloudFormation to streamline and automate deployment. In addition to achieving high availability, these components of the AWS Global Infrastructure can help your business achieve benefits like elasticity and agility.

- Going global with AWS infrastructure
The coffee shop is expanding to global locations. Navigate through the following content to review how elements of our coffee shop expansion represent different parts of the AWS Global Infrastructure.

- How to choose a Region or set of Regions
If we were to expand our coffee shop by opening new locations, there would be multiple things to consider, like customer demand and development cost. Similarly, you have several factors to consider when selecting a Region or set of Regions for your real-life resources.

- AWS edge locations

- Like our coffee franchise could expand with smaller versions of the shop such as mobile coffee carts, AWS has smaller footprint facilities called edge locations. Edge locations cache items like images, videos, and other resources, so that users can access the content they need with lower latency.
Edge locations, on the other hand, are part of the AWS content delivery network (CDN). They are optimized for content delivery, not directly tied to Availability Zones.

- Infrastructure as code and CloudFormation
Another important consideration of a coffee shop expansion would be to maintain a consistent product from location to location. AWS has services, such as CloudFormation, that you can use to help automate the deployment of your cloud resources. These services use infrastructure as code, or IaC, helping you achieve a consistent, reliable set up each time your business grows.

- Key considerations when choosing Regions

- Compliance
Compliance is an important consideration when selecting Regions for deploying business resources. Different geographical locations have varying regulatory requirements and data protection laws that organizations must follow. For example, the General Data Protection Regulation (GDPR) is designed to protect the personal data and privacy of individuals within the European Union (EU). An online retail company operating in the EU would be required to meet GDPR compliance to protect customer data. GDPR compliance includes obtaining proper consent for data collection and providing mechanisms for data access and deletion.

- Proximity
When selecting a Region, you also want to consider how to achieve low latency for your users. Regions closer to your user base minimize data travel time, which reduces latency and enhances application responsiveness. Choosing a Region or set of Regions farther away from customers could introduce delays, which might impact user satisfaction and overall system efficiency.

- Feature availability
You also want to consider which specific features and services are available in each Region. AWS is constantly expanding features and services to multiple locations, but not all Regions contain all AWS offerings. For example, AWS GovCloud Regions are specifically designed to meet the compliance and security requirements of US government agencies and their contractors. These Regions have stringent physical, operational, and personnel security controls in place. These controls are only available in specific Regions to meet certain governmental regulatory requirements.

- Pricing
When selecting a Region, pricing is also a factor that can influence your decision. Some Regions have lower operational costs than others. These operational costs can impact the overall expenses for hosting applications and services. Tax laws and regulations can also play a role in cost. Some Regions might offer tax incentives or have lower tax rates, which can affect customer pricing. Additionally, data sovereignty laws in certain Regions might require data to be stored locally, affecting both compliance and cost.

- Edge locations, another important component of the AWS Global Infrastructure landscape. Edge locations
Edge locations are strategically placed sites around the world that cache content to deliver data, video, and applications with lower latency and higher transfer speeds. Edge locations are considered a vital part of the AWS content delivery network (CDN) and use services like CloudFront to efficiently distribute data to end users.

- Relationship between Regions, Availability Zones, and edge locations, choose each of the three numbered markers.
Region(Regions are geographical areas around the world that are made up of multiple data center)->3 or more Availability zones(AZs)-> 1 or more DataCenters

- Regions are geographical areas around the world that are made up of multiple data centers. These data centers provide scalable and redundant infrastructure for hosting cloud services. Each Region consists of multiple, isolated locations known as Availability Zones. Each Region has three or more Availability Zones.

- Availability Zones are distinct locations within a Region, each designed as an independent zone with its own power, networking, and connectivity. Availability Zones maintain high availability and fault tolerance for applications. Each Availability Zones consists of one or more data centers.

- Interacting with AWS resources
As you've learned, there are a number of ways you can operate in the AWS Cloud. To interact with AWS resources, you must invoke AWS APIs. To interact with these APIs, you can use the AWS SDKs, the AWS Command Line Interface (AWS CLI), the AWS Management Console, or IaC tools such as CloudFormation. To review functions and use cases for using these approaches, choose each of the numbered markers.

- CloudFormation(aws IaC)
CloudFormation is a service that helps you model and set up your AWS resources so that you can spend less time managing those resources and more time focusing on your applications that run in AWS. With CloudFormation, you can define your infrastructure as code. You create a template that describes all the AWS resources that you want (like Amazon Elastic Compute Cloud (Amazon EC2) instances), and CloudFormation takes care of provisioning and configuring those resources for you.

- Edge locations, on the other hand, are part of the AWS content delivery network (CDN). They are optimized for content delivery, not directly tied to Availability Zones.

- When deciding where to place cloud resources, companies must consider multiple factors. Compliance refers to the Region meeting legal or regulatory requirements. Proximity to customers helps reduce latency and improve user experience. Feature availability makes sure that the required AWS services are supported in the chosen Region. Pricing varies by Region, so cost-efficiency is also a critical factor.

---

## Introduction to Networking

- Describe what a virtual private cloud (VPC) is and what it does.
Describe what a subnet is and what it does.
Describe the difference between a public and private subnet.

- The term networking refers to interconnected devices that can exchange data and resources. Networking in the AWS Cloud consists of the infrastructure and services working together to host your applications, data, and any other resources you might need. Let's get started and learn about the foundational network components used in the AWS Cloud.

- Amazon Virtual Private Cloud (Amazon VPC)
An Amazon VPC lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define.

- Subnet
Subnets are used to organize your resources and can be made publicly or privately accessible. A private subnet is commonly used to contain resources like a database storing customer or transactional information. A public subnet is commonly used for resources like a customer-facing website.

- Define what a virtual private gateway is and what it does.
Identify the core components of a VPC.
Define an internet gateway and what it does.

- Amazon VPC
With Amazon VPC, you can provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. It provides three main benefits. It helps increase security because you can secure and monitor connections, screen traffic, and restrict instance access. Amazon VPC gives you full control over your resource placement, connectivity, and security. The convenience of using Amazon VPC means you will spend less time setting up, managing, and validating your virtual network when compared to on-premises network management.

- Subnets
Within an Amazon VPC, you can organize your resources into subsections or subnets. A subnet is a section of an Amazon VPC that can contain resources, such as Amazon EC2 instances. You will learn more about subnets in the next lesson.

- Connecting your resources with an internet gateway
To allow public traffic from the internet to access your VPC, you attach an internet gateway to the VPC. An internet gateway is a connection between a VPC and the internet. You can think of an internet gateway as being similar to a doorway that customers use to enter the coffee shop. Without an internet gateway, no one can access the resources within your VPC.

- Virtual private gateways
What if you have a VPC that includes only private resources? The following example shows how a virtual private gateway works. You can think of the internet as the road between your home and the coffee shop. It is open and accessible to anyone. You want a way to protect the traffic you send on the internet from the public, internet service providers, and others who might be trying to track or intercept it. This is where a virtual private network (VPN) connection comes in.

- VPN creates a connection that is more like a secure tunnel through the internet. Using encryption, it hides and protects everything you send and receive from outside eyes. A virtual private gateway is the component in the AWS Cloud that makes it possible for you to connect this protected traffic to enter the VPC. With a VPN connection, your data travels privately and safely, hidden from others using the same route.

- With a virtual private gateway, you can establish a VPN connection between your VPC and a private network, such as an on-premises data center or internal corporate network. A virtual private gateway allows traffic into the VPC only if it is coming from an approved network.

- Amazon Virtual Private Cloud(VPC)
Amazon VPC is used to establish boundaries around your AWS resources.

- Virtual private gateway
A virtual private gateway allows protected internet traffic to enter into the VPC.

- Virtual private network(VPN)
A VPN encrypts your internet traffic, helping protect it from anyone who might try to intercept or monitor it.

- With so many different types of networks, on-premises datacenters, and remote workers, companies need a wide range of ways to connect to the AWS Cloud. In the following section, you will learn four ways to connect to the AWS Cloud:
AWS Client VPN
AWS Site-to-Site VPN
AWS PrivateLink
AWS Direct Connect

- AWS Client VPN
AWS Client VPN is a networking service you can use to connect your remote workers and on-premises networks to the cloud. It is a fully managed, elastic VPN service that automatically scales up or down based on user demand. Because it is a cloud VPN solution, you don’t need to install and manage hardware or try to estimate how many remote users to support at one time.

- Benefits: AWS Client VPN provides advanced authentication, remote access. It is elastic and fully managed.

- Use case: It can be used to quickly scale remote-worker access.

- Client VPN, a managed VPN service, provides secure access to AWS resources and on-premises networks from anywhere. It uses an OpenVPN-based client, and it works with global Regions by using the AWS global network.

- Securely connect sites to other sites
Some companies might want to establish secure, encrypted connections between their on-premises networks like data centers or branch offices and their resources in their Amazon VPC. That's where Site-to-Site VPN can help.

- AWS Site-to-Site VPN
Site-to-Site VPN creates a secure connection between your data center or branch offices and your AWS Cloud resources.

- Benefits: Site-to-Site VPN provides high availability, secure and private sessions, and accelerates applications.

- Use cases: It can be used for application migration and secure communication between remote locations.

- AWS Cloud with a VPN and resources with a virtual private gateway. The branch office, data center, and manufacturing site are connecting with secure VPN connections.

- Securely connect resources, even in other VPCs
Other companies sometimes need the flexibility to privately connect to resources in other cloud providers as though they were in their own VPC. They need a way to communicate with these resources and don't want the hassle of setting up gateways or site-to-site VPNs. That's where AWS PrivateLink can help.

- AWS PrivateLink
AWS PrivateLink is a highly available, scalable technology that you can use to privately connect your VPC to services and resources as if they were in your VPC. You do not need to use an internet gateway, NAT device, public IP address, Direct Connect connection, or AWS Site-to-Site VPN connection to allow communication with AWS services or resources from your private subnets. Instead, you control the specific API endpoints, sites, services, and resources that are reachable from your VPC.

- Benefits: AWS PrivateLink helps you secure your traffic and connect with simplified management rules.

- Use case: It is used for connecting your clients in your VPC to resources, other VPCs, and endpoints.

- Even though the preceding connections are highly available and scalable, traffic jams are possible because you’re using the same connection as other clients. That's why for some use cases, you might need a dedicated private connection with a lot of bandwidth.

- Dedicated private connections for increased bandwidth

- AWS Direct Connect
Direct Connect is a service that makes it possible for you to establish a dedicated private connection between your network and VPC in the AWS Cloud.

- Benefits: AWS Direct Connect reduces network costs and increases amount of bandwidth.

- A corporate data center routes network traffic to an AWS Direct Connect location. That traffic is then routed to a VPC through a virtual private gateway. All network traffic between the corporate data center and VPC flows through this dedicated private connection.

- To learn more about Direct Connect, expand each of the following three categories.

- latency sensitive apps
Direct Connect bypasses the internet and provides a consistent, low-latency network experience. This makes it ideal for applications like video streaming and other real-time applications that require high performance.

- Large scale data migration or transfer
Direct Connect helps ensure smooth and reliable data transfers at massive scale for real-time analysis, rapid data backup, or broadcast media processing.

- Hybrid cloud architecture
You can use Direct Connect to link your AWS and on-premises networks to build applications that span environments without compromising performance.

- Additional gateway services
There are several different types of gateways you can use to connect your AWS resources. Depending on your needs, you might want to learn more about what they are used for and where to go to learn more. To learn more about these additional gateway types, expand each of the following three categories.

- AWS Transit Gateway is used to connect your Amazon VPCs and on-premises networks through a central hub. As your cloud infrastructure expands globally, inter-Region peering connects transit gateways together using the AWS Global Infrastructure. To learn more, refer to AWS Transit Gateways(opens in a new tab).

- A NAT gateway is a NAT service. You can use a NAT gateway so that instances in a private subnet can connect to services outside your VPC but external services can't initiate a connection with those instances. To learn more, refer to NAT gateway(opens in a new tab).

- You learned about Application Programming Interface (API)s earlier. Quick refresher, an API defines how different software systems can interact and communicate with each other. The Amazon API Gateway is an AWS service for creating, publishing, maintaining, monitoring, and securing APIs at any scale. To learn more, refer to Amazon API Gateway(opens in a new tab).