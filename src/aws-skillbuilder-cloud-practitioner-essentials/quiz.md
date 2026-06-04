## QUIZ Module 1 - Introduction to the Cloud

> Q: Which scenario BEST describes how the client-server model works in coffee-shop analogy?
> 
> A: The customer goes to the barista and places an order for a coffee. The barista prepares the coffee and hands it back to the customer. This describes how the client places the request, and the server responds.
---

> Q: Which deployment model balances compliance (on-premises) and scalability (cloud)?
> 
> A: Hybrid deployment

---

> Q: A retail business plans to launch a new line of clothing but struggles with predicting the server capacity needed for the launch. Which AWS Cloud benefit helps address this challenge?
>
> A: Stop guessing capacity

---

> Q: How does AWS Global Infrastructure ensure high availability?
>
> A: AWS provides multiple data centers across different geographic regions, so your website remains operational even if one location experiences issues.

---

> Q: Which party is responsible for applying security patches to the OS that is running in the cloud?
>
> A: Your company is responsible for applying security patches to the OS.

**ASSESSMENT:**

> Q: A finance company is interested in migrating to the cloud and is curious about who is responsible for securing the physical infrastructure of the cloud.
>
> A: AWS is responsible for securing the physical infrastructure, and the company can focus on securing their data and applications within the cloud.

---

> Q: A global web application needs to ensure performance and reliability by using AWS infrastructure. What are the key advantages of AWS infrastructure to meet these needs?
>
> A: 
>   - High availability 
>   - Fault tolerance.

---

> Q: A cloud architect explains the customer's responsibilities under the AWS Shared Responsibility Model. What responsibilities does the customer have in this model?
>
> A: Managing OS patches / Encrypting client-side data.

---

> Q: A small business is concerned about fixed costs when considering migrating its IT infrastructure to the cloud. How does cloud computing address this concern?
>
> A: Cloud computing is a model for delivering IT resources over the internet. Businesses can rent services on a pay-as-you-go basis, which can help reduce fixed costs and allow for more flexible budgeting.

---

> Q: Your team lead has asked you to explain the client-server model and how cloud computing fits into this model. What is the best explanation?
>
> A: In the client-server model, the client sends requests to the server, which processes the requests and sends back responses. Cloud computing provides scalable server resources that can be accessed over the internet.

---

> Q: A large enterprise is looking to lower operational costs by reducing the overhead associated with managing its infrastructure. What is a key advantage of cloud computing in this case?
>
> A: Stop spending money running and maintaining data centers.

---

> Q: A government agency wants to maintain complete control over its IT infrastructure but plans to use AWS Cloud services for specific applications. Which deployment model is suitable for their needs?
>
> A: Hybrid deployment.

---

> Q: Your company is expanding globally and needs high availability. What is the difference between AWS Regions and Availability Zones?
>
> A: A Region is a geographical location that contains three or more Availability Zones. An Availability Zone is a distinct location within a Region that contains one or more discrete data centers.

---

## QUIZ Module 2 - Compute in the Cloud


> Q: How does EC2 compare to running servers on premises?
>
> A:  It is more flexible, cost-effective, and quicker to get started

> Q: What is multi-tenancy in the context of EC2 instances
>
> A: Each vm is isolated but shares resources from a host machine.

> Q: A company uses EC2 instance to deploy their application, what whould happen if they need to stop or terminate the EC2 instances?
>
> A: You pay only for running instances, not for stopped ord terminated ones.

> Q: What must be specified when preparing to launch an EC2 instance?
>
> A: The types of instance and the OS

--- 
> Q: Which Amazon EC2 instance type is best suited for fast real-time analytics of large datasets?
>
> A: Memory optimized

> Q: Which Amazon EC2 instance type is best suited for fast, consistent access to large locally stored datasets?
>
> A: Storage Optimized

---
> Q: What is a primary advantage of using the AWS CLI over the AWS Management Console?
>
> A: It uses automation and scripting, which reduces manual steps and errors.

> Q: What is the customer's responsibility when using compute services like EC2 according to the AWS shared responsibility model?
>
> A: The customer is responsible for configuring, securing, and managing the OS, networking, and applications on their EC2 instances.

---

> Q: What are the required configurations when launching an Amazon EC2 instance for a web server (3)
>
> A: Amazon Machine Image (AMI) / Instance type / Storage

> Q: What is an Amazon Machine Image (AMI) used for when launching an Amazon EC2 instance
>
> A: To pre-configure the OS and software

---

> Q: How can a financial services company run sensitive, regulation-compliant applications with full control over physical server placement and resource allocation?
>
> A: Dedicated Hosts

> Q: How can a startup reduce costs for an interruptible batch processing workload by using unused Amazon EC2 capacity?
>
> A: Spot Instances

> Q: How can a customer build a new application with uncertain usage patterns and future growth without making a long-term commitment?
>
> A: On Demand

---

> Q: What is the primary benefit of scalability and elasticity in AWS
>
> A: The ability to grow and shrink resources dynamically based on real-time demand

> Q: What is the main reason for deploying Amazon EC2 instances across multiple Availability Zones?
>
> A: To provide high availability by allowing instances in different Availability Zones to handle traffic if one Availability Zone fails

> Q: How does AWS make sure that a business can meet fluctuating demand without over-provisioning resources?
>
> A: By allowing businesses to provision resources that automatically scale based on demand

---

> Q: How does Elastic Load Balancing (ELB) improve scalability in AWS?
>
> A: It automatically routes traffic to instances based on various routing methods.

> Q: Which task does Elastic Load Balancing (ELB) perform?
>
> A: Distributes a workload across several Amazon EC2 instances.

---

> Q: What BEST describes the key difference between tightly coupled and loosely coupled architectures?
>
> A: In a tightly coupled architecture, components are tightly connected and dependent on each other, whereas in a loosely coupled architecture, components can operate independently.

> Q: In a banking system, when customers transfer money, the transaction details are sent from the transaction service to a fraud detection service for verification. Sometimes, the fraud detection service is temporarily down.
>
> What is the MAIN advantage of using Amazon Simple Queue Service (Amazon SQS) in this banking scenario?
>
> A: It stores transaction details until the fraud detection service can process them, even if the service is down.


**ASSESSMENT:**


> Q: What does multi-tenancy refer to in the context of Amazon EC2?
>
> A: Multiple users sharing the same EC2 instance while maintaining isolation

> Q:A university research team is running climate modeling simulations that require substantial CPU power to process complex algorithms and analyze large datasets.
>
> Why are compute optimized Amazon EC2 instances ideal for this task?
>
> A: They are ideal for tasks that require significant CPU power to perform computations.

> Q: How do Amazon EC2 Auto Scaling and Elastic Load Balancing (ELB) work together in AWS?
>
> A: Amazon EC2 Auto Scaling adjusts the number of instances, whereas ELB distributes traffic evenly across them.

> Q: A manufacturing company is running a set of predictable workloads for the next 3 years and wants to optimize costs.
>
> Which option should they choose?
>
> A: Reserved Instances

> Q: A software development company needs to notify the engineering team whenever a new bug is reported in their bug tracking system. Some team members need to be notified immediately, whereas others can process the bug reports later.
>
> Which service should the software development company choose based on the requirements?
>
> A: Amazon Simple Notification Service (Amazon SNS)

> Q: Which tool can be used to interact with AWS services through a graphical user interface (GUI)?
>
> A: AWS Management Console

> Q: What is the primary role of an Amazon Machine Image (AMI) when scaling applications?
>
> A: It provides a consistent image to launch new instances.

> Q: A media company is working on a project that involves rendering complex visual effects and simulations. The rendering process requires significant computational power and hardware accelerators to handle the intense workload efficiently.
>
> Which Amazon EC2 instance type would be the BEST choice for this task?
>
> A: Accelerated computing

> Q: A marketing agency is developing a new web application and expects steady growth, but is unsure of traffic in the early months. They want flexibility without a long-term commitment.
>
> Which pricing option should they use?
>
> A: On-Demand

> Q: A startup company is building a new web application and chooses general purpose Amazon EC2 instances to host the application.
>
> Why did they choose this instance type?
>
> A: It provides a balanced mix of compute, memory, and networking resources while keeping costs efficient as they scale their user base.

> Q: A company has critical steady-state workloads and batch jobs that are not time-sensitive.
>
> How should they optimize costs using Amazon EC2 Savings Plans and Spot Instances?
>
> A: Use Savings Plans for critical workloads and Spot Instances for jobs that are not time-sensitive to maximize savings.

> Q: How does Amazon EC2 Auto Scaling work in AWS?
>
> A: Amazon EC2 Auto Scaling automatically adds or removes instances based on performance data and application metrics.

> Q: What happens if one component fails in a loosely coupled architecture?
>
> A: The system can continue to function as other components are independent.

> Q: Which option BEST describes how compute resources are provisioned and managed in the cloud?
>
> A: Resources are provisioned based on demand, allowing for scaling and management.

---

## QUIZ Module 3 - Exploring Compute Service


> Configure operating system, security patches, and network settings - UNMANAGED
>
> Choose deployment options and configure environment settings - MANAGED
>
> Focus only on writing and deploying code - FULLY MANAGED

---

> Q:A development team at a fintech startup is building a new customer-facing microservice using AWS Lambda. AWS takes care of the infrastructure, but the team is focused on meeting strict security and compliance requirements.
>
> Which task is still the team's responsibility when using Lambda?
>
> A: Managing data access permissions


> Q: A photography company offers cloud-based photo editing and storage. To streamline operations, it uses AWS Lambda to automatically process photos—resizing images, applying filters, and organizing files—every time a client uploads a new image.
>
> Which key components are involved in running an automated photo processing workflow with Lambda? (3)
>
> A: Lambda function / Triggers / Runtimes

---

> Q: A developer just finished building an application that runs flawlessly on their laptop. However, when their team tries to deploy it in a different environment, it crashes because of missing dependencies and configuration mismatches.
>
> How do containers help solve this problem?
>
> A: By packaging the application and everything it needs to run into one consistent environment

> Amazon Elastic Container Service (Amazon ECS) - Scalable container orchestration service for running containers on AWS
>
> Amazon Elastic Kubernetes Service (Amazon EKS) - Fully managed Kubernetes service for deploying and scaling containers
>
> Amazon Elastic Container Registry (Amazon ECR) - Stores, manages, and deploys Open Container Initiative (OCI)-compliant container images
>
> AWS Fargate - Serverless compute engine for containers—removes the need to manage servers

---

> AWS Elastic Beanstalk - A managed service for deploying and scaling web applications
>
> AWS Batch - A fully managed service for batch computing workloads
>
> Amazon Lightsail - A simplified service with virtual private servers (VPSs), storage, and networking
>
> AWS Outposts - A hybrid cloud service extending AWS to on premises

> Q: A startup is building a web application and wants a simple way to deploy code without managing infrastructure. They need to have auto scaling and monitoring handled for them.
>
> Which AWS service should they use?
>
> A: AWS Elastic Beanstalk

> Q: A financial company must run workloads on premises because of strict compliance requirements, but it wants to use AWS services and tools consistently across environments.
>
> Which service meets their needs?
>
> A: AWS Outposts


**ASSESSMENT:**


> Q: A developer is launching a new microservice and wants to focus only on writing and deploying code. They do not want to manage servers, handle scaling, or worry about infrastructure availability.
>
> Which AWS service model is BEST for this use case?
>
> A: Serverless

> Q: A development team at a travel company has stored their hotel booking system’s container image in Amazon Elastic Container Registry (Amazon ECR) and is ready to deploy it. They need a service that can automatically start and stop containers based on traffic, scale up or down with demand, and monitor the health of the system.
>
> Which service does the team need next?
>
> A:  An orchestration service like Amazon Elastic Container Service (Amazon ECS) or Amazon Elastic Kubernetes Service (Amazon EKS)

> Q: Which scenario is the BEST fit for using AWS Lambda?
>
> A: Automatically processing images as users upload them to an Amazon S3 bucket

> Q: A company is launching a containerized photo application and has built the container image, which needs to be stored securely. They plan to use Kubernetes for orchestration and prefer not to manage any servers.
>
> Which combination of AWS services BEST fits their needs?
>
> A: Amazon Elastic Container Registry (Amazon ECR), Amazon Elastic Kubernetes Service (Amazon EKS), and AWS Fargate

> Q: A development team at an e-commerce company is working on a new website. The application runs fine on their local machines, but when they attempt to deploy it to a staging environment, it does not work as expected. The team wants to make sure that the application runs consistently across all development, testing, and production environments going forward.
>
> Which solution should the team use to make sure that the application runs the same across all environments?
>
> A: Package the application in a container that includes all dependencies.

> Q: A pharmaceutical research company needs to run thousands of simulations to analyze protein folding. These compute-heavy tasks are run in parallel and do not require real-time interaction. The company wants the jobs to be automatically scheduled and scaled based on computing demand.
>
> Which AWS service BEST fits this workload?
>
> A: AWS Batch

> Q: A freelance developer is building a blog for a client with minimal traffic. They want a basic, cost-effective solution that includes storage and compute in one package, without having to deal with complex configurations or scaling concerns.
>
> Which AWS service is the BEST fit?
>
> A: Amazon Lightsail

> Q: What is the customer responsible for managing in a serverless service like AWS Lambda?
>
> A: The application code


---

## QUIZ Module 4 - Going Global


> Q: A cloud engineer for a government agency is tasked with selecting an AWS Region to deploy the agency's resources.
>
> Which factors are MOST important to consider when selecting a Region? (Select TWO.)
>
> A: Any regulatory compliance standards the agency requires / Proximity to users

---

> AWS Region - A Physical location around the world where AWS operates multiple data centers
>
> Availability Zone - Separate, distinct locations with one or more data centers that are engineered to be isolated from failures in other areas
>
> Edge location - Locations that cache content to deliver data, video, and applications to users with lower latency

---

> Q: A rapidly growing tech startup company is planning to launch a new web application that will require a complex infrastructure setup, including multiple Amazon EC2 instances, Elastic Load Balancing, and Auto Scaling groups. The application must be deployed consistently across different environments.
>
> Would AWS CloudFormation be a good solution for managing the company's infrastructure?
>
> A: CloudFormation would be ideal because it supports infrastructure as code (IaC), enabling consistent, repeatable deployments across different environments.
>
> _CloudFormation is designed to handle complex infrastructure setups. It defines infrastructure as code to help make sure that deployments are consistent across different environments such as development, testing, and production._


**ASSESSMENT:**


> Q: Which answer BEST describes the purpose and benefits of AWS edge locations?
>
> A: Edge locations cache content to deliver data with lower latency and higher transfer speeds to end users.


> Q: Which answer describes the key features and benefits of AWS CloudFormation?
>
> A: With CloudFormation, users can model and set up their AWS resources using code to automate provisioning and the management of infrastructure. This method can help to reduce errors and maintain consistency across environments.


> Q: What BEST describes key benefits of using multiple AWS Regions and multiple Availability Zones? (Select TWO.)
>
> A: High availability and fault tolerance /  Low latency for end users
>
> _By using multiple AWS Regions, a company can place their resources closer to their end users, which reduces the distance that the data must travel. This results in lower latency and a better user experience. By using multiple Availability Zones within a Region, the company enhances the fault tolerance of their applications. If one zone fails, their application can continue to operate from another zone, maintaining high availability._


> Q: A team at a biomedical tech company is tasked with deploying a new medical application across multiple AWS Regions to help maintain high availability and fault tolerance. The application consists of several components, including a web server, a database, and a message queue. The deployment needs to be consistent and repeatable and should minimize manual errors through automation.
>
> Which approach is BEST suited for deploying this application according to the needs of automation and consistency?
>
> A: Using an Infrastructure as Code (IaC) service such as AWS CloudFormation to deploy the application


> Q: Which answer BEST describes the relationship between AWS Regions, Availability Zones, and edge locations?
>
> A: AWS Regions are physical locations around the world where AWS has multiple Availability Zones. Edge locations are located outside of AWS Regions and cache frequently accessed content.


> Q: A nonprofit organization is migrating all of their resources to the AWS Cloud. They are trying to decide which AWS Region to deploy their resources to.
>
> Which option lists the factors the organization needs to consider when deciding where to place their cloud resources?
>
> A: Compliance, proximity to customers, feature availability, and pricing
>
> _When deciding where to place cloud resources, companies must consider multiple factors. Compliance refers to the Region meeting legal or regulatory requirements. Proximity to customers helps reduce latency and improve user experience. Feature availability makes sure that the required AWS services are supported in the chosen Region. Pricing varies by Region, so cost-efficiency is also a critical factor.__

---

## QUIZ Module 5 - Networking

> Q: What are the uses of a subnet in an Amazon VPC? (Select THREE.)
>
> A: Can be used to share public resources / Can be used to isolate resources and keep them private / Can be used to organize your resources

---

> Q: A company is setting up their Amazon VPC. They need to connect their corporate data center through the internet with a secure connection. They also want to make sure the resources are isolated from the public.
>
> Which solution would BEST meet their needs?
>
> A:  A virtual private gateway with a VPN connection and a private subnet in the Amazon VPC

---

> Q: A company is conducting a large-scale migration of their on-premises data center with their data warehouse and data backup. They need a solution that will meet the large amount of bandwidth requirements during migration. The solution will also be used for their ongoing data transfers after the move because they will retain part of their on-premises data center for a hybrid cloud solution.
>
> Which AWS solution would best meet their needs?
>
> A: AWS Direct Connect link to their on-premises network and the AWS Cloud

> Q: A company is choosing the type of gateway for their network. They need to connect their corporate data center with their private subnet in their Amazon Virtual Private Cloud. Their gateway needs to allow only protected internet traffic to enter into the Amazon VPC. It should also allow a connection between their Amazon VPC and a private network only if it is coming from an approved network.
>
> Which type of gateway would BEST meet their needs?
>
> A: Virtual private gateway

---

> Q: A retail customer is setting up their application in the AWS Cloud. The application requires a lot of control in defining traffic rules for the individual Amazon EC2 instances in their public subnet.
>
> Which solution would BEST meet the requirements for securing the resources?
>
> A: Set up security groups for the EC2 instances based on the application requirements.

> Q: Which network component performs stateless packet filtering?
>
> A: Network access control list (network ACL)

---

> Q: An enterprise customer with a worldwide sales force is looking to deliver their large library of sales training content. They want to make sure their sales force can access the media-rich training content with low latency and reduced costs.
>
> Which AWS service would BEST fit the customer's need?
>
> A:  Amazon CloudFront

> Q: After years of working with different domain registration companies, a media company is looking for a solution to manage all their existing domain names. They also want to register new domain names. Ideally, they would like to manage all their domain names in a single service.
>
> Which AWS service would BEST fit the customer's need?
>
> A: Amazon Route 53

---

> Q: A healthcare company is looking to create a dedicated network connection to AWS. They would use this connection for their heavy payloads of data being sent over the internet to AWS. They also have compliance requirements due to the sensitive nature of their patient data.
>
> Which type of connection to the AWS Cloud would BEST meet their needs?
>
> A: AWS Direct Connect connection from their corporate data center to a virtual private gateway in their VPC in the AWS Cloud

---

ASSESSMENT


> Q: What is the primary function of a domain name service (DNS)?
>
> A: It translates human-readable domain names to machine readable IP addresses.

> Q: A customer is creating an Amazon VPC for their application. They want to create a private segment in the Amazon VPC so that resources launched can be isolated from users on the internet.
>
> Which network component would BEST meet their needs?
>
> A: A private subnet

> Q: A financial customer needs a content delivery solution to deliver required training videos and static content to their financial consultants worldwide. They want to make sure the solution provides low latency.
>
> Which AWS solution would BEST meet their needs?
>
> A: Amazon CloudFront

> Q: An enterprise customer just merged with another company and needs a way to quickly scale and provide a way for the new worldwide sales force to access their AWS resources. They want a fully managed service with advanced authentication for their new remote workers.
>
> Which solution would BEST meet their needs?
>
> A: AWS Client VPN

> Q: What is networking in the AWS Cloud?
>
> A: Interconnected devices that can exchange data and resources????

> Q: A customer is exploring solutions to establish secure, encrypted connections between their on-premises networks at their data centers and branch offices. They are looking for the MOST cost-effective way to connect their office sites to other sites and their AWS services. They are not looking to increase the amount of bandwidth.
>
> Which solution would BEST meet their needs?
>
> A: AWS Site-to-Site VPN

> Q: A customer is creating their application resources in their virtual private cloud (VPC) subnets. They want to secure their resources in the cloud, specifically the networking traffic protection tasks.
>
> Which component is the customer responsible for, based on the shared responsibility model?
>
> A: Securing network traffic with the subnets and resources with Network access control lists (network ACLs) and security groups

> Q: What is the primary function of an Availability Zone in the AWS Cloud?
>
> A: It enhances application availability and fault tolerance by allowing resources to be deployed across multiple zones.

> Q: A customer wants a way to establish a dedicated connection from their on-premises network to an Amazon VPC. They need a solution that provides a more consistent network experience with increased bandwidth.
>
> Which type of connection to the AWS Cloud would BEST meet their needs?
>
> A: AWS Direct Connect

> Q: A retail customer is hosting their application in an Amazon VPC and wants to configure traffic rules for the Amazon EC2 instances running in a public subnet. The application requires multiple rules to be defined at the instance level.
>
> Which solution or feature would meet their needs?
>
> A: Set up security groups for the Amazon EC2 instances based on the application requirements.

> Q: A company wants to establish a secure, private connection between their on-premises data center and their Amazon VPC to create a hybrid cloud architecture.
>
> Which component should they use to help ensure a secure connection?
>
> A: Virtual private gateway
>
> _A virtual private gateway is the virtual private network (VPN) endpoint on the AWS side. It provides a way for you to establish a secure, encrypted connection between your on-premises network and your virtual private cloud (VPC)._

> Q: A customer is moving their application to an Amazon VPC and wants to setup a traffic control at the subnet level. They need broad control of traffic in and out and would like to use both allow and deny type rules.
>
> Which solution or feature would meet their needs?
>
> A: Use network access control lists (network ACLs).

> Q: A customer is exploring edge networking services to improve application availability, performance, and security. They need a solution for traffic routing when something goes wrong in one of their application's locations. Specifically, it takes into account the endpoint health, user location, and policies.
>
> Which AWS solution would BEST meet their needs?
>
> A: AWS Global Accelerator

> Q: A media company needs a service to manage their domain registrations with different providers. They will also be using the service to route internet traffic to their resources hosted both in the AWS Cloud and elsewhere.
>
> Which AWS solution would BEST meet their needs?
>
> A: Amazon Route 53 

---

## QUIZ Module 6 - Storage

> Q: A developer is building an application that processes large amounts of data and requires high I/O performance. After processing the data for an operation, the results are displayed to the user and do not need to be retained long-term. Unfortunately, the application's current storage solution is experiencing performance bottlenecks during peak processing times.
>
> How could implementing an EC2 instance store improve the performance of the application?
>
> A: EC2 instance store provides high I/O performance for temporary storage needs.

> Q: AnyCompany Finance is designing an application that requires consistent and low-latency access to financial data. They're looking for a storage solution that provides persistent block storage.
>
> Why would Amazon EBS be suitable to store data in this scenario?
>
> A: Amazon EBS provides high availability and durability by automatically replicating volumes within the same Availability Zone.

> Q: AnyCompany Software is migrating their on-premises application architecture to AWS. They are particularly concerned about data persistence because in their current environment, they have experienced data loss when virtual machines (VMs) crashed. They want to understand how Amazon Elastic Block Store (Amazon EBS) can help address their data persistence requirements when they move their workloads to Amazon EC2 instances.
>
> How does Amazon EBS solve the data persistence issue described in this scenario?
>
> A: Amazon EBS volumes exist independently from the instance and persist even after the instance is terminated.

---

> Q: AnyCompany Commerce operates an online trading platform experiencing rapid growth. Their development team frequently needs to create test environments that mirror production for testing new features, but setting up these environments has become time-consuming and error-prone.
>
> What is the most significant benefit of using EBS snapshots in this scenario?
>
> A: EBS snapshots enable rapid creation of new volumes from existing data, so you can quickly deploy identical test environments that mirror production.

> Q: AnyCompany Healthcare manages thousands of EBS volumes containing patient records. They need to ensure that this data is properly backed up, retained according to compliance requirements, and old snapshots are removed to control costs.
>
> Which problem does AWS Data Lifecycle Manager primarily solve in this scenario?
>
> A: Automating the creation, retention, and deletion of EBS snapshots and EBS backed Amazon Machine Images (AMIs) according to a schedule

---

> Q: AnyCompany Mobile is evaluating cloud storage solutions for their new mobile application. They need a reliable service that can handle various types of data storage requirements as their user base grows.
>
> Based on this scenario, what is an aspect of Amazon S3 that they could use in this scenario?
>
> A: Storing and distributing mobile application content and user-generated media files

> Q: AnyCompany Marketing has created an Amazon S3 bucket to host images for their new website. The images need to be accessible to anyone visiting the website without authentication. After uploading the images to the bucket, users report they cannot access them, even though the bucket policy is set to allow public access.
>
> What is the most likely cause of this access issue?
>
> A: Block public access settings are enabled at the account or bucket level.

> Q: AnyCompany Media is looking for a new cloud storage solution. They distribute large video files to users around the world, and are looking for a service that is highly durable, scalable, and offers various access control mechanisms.
>
> Based on this scenario, which Amazon S3 feature would be particularly beneficial?
>
> A: Amazon S3 offers 99.999999999 percent (11 nines) of durability for objects stored across multiple Availability Zones. This maintains highly available for their video content and protects it against data loss.

---

> Q: AnyCompany Business stores a growing amount of customer data in Amazon S3. Their manager is concerned about storage costs and asks IT to implement a solution to move older data to cheaper storage. The data is frequently accessed for the first 30 days, occasionally accessed for the next 60 days, and rarely accessed after 90 days.
>
> What should they do in this situation to optimize costs while maintaining appropriate access to the data?
>
> A: Create a lifecycle rule to transition objects to S3 Standard-Infrequent Access (S3 Standard-IA) after 30 days, transition to S3 Glacier after 90 days.

> Q: Which statement BEST describes S3 Lifecycle?
>
> A: A feature used to define rules to automatically transition objects between different storage classes, or delete them based on age or usage patterns.

---

> Q: AnyCompany Financial needs to implement a new data application that will analyze market data. The application must be able to scale compute resources up or down to match traffic demand while maintaining access to the same datasets.
>
> What is a benefit of using Amazon EFS as the storage solution for the application described in this scenario?
>
> A: Amazon EFS provides elastic storage capacity, automatically scaling up and down as files are added and removed, with no disruption to applications.

> Q: AnyCompany Retail is planning to migrate their on-premises file storage to AWS. They need a solution that allows their global development teams to collaborate on the same set of files simultaneously.
>
> Which feature of Amazon EFS makes it a good fit for this scenario?
>
> A: Amazon EFS provides shared access for thousands of Amazon EC2 instances, with consistent low latencies.

---

> Q: AnyCompany Media wants to migrate its file shares to AWS while maintaining compatibility with existing applications. They need a solution that supports Server Message Block (SMB) protocol and integrates with Microsoft Active Directory.
>
> Which AWS service should they implement in this scenario?
>
> A: Amazon FSx for Windows File Server

---

> Q: AnyCompany has a large collection of files stored on-premises that needs to be backed up to the AWS Cloud. They want to maintain local access to frequently used files while using cloud storage for cost savings. They also want to minimize changes to their existing file-sharing workflows and applications.
>
> Which AWS Storage Gateway type BEST addresses these requirements?
>
> A: Amazon S3 File Gateway

> Q: AnyCompany Manufacturing stores CAD files that need to be accessed frequently by engineers at their on-premises data center. They want to maintain local access to this data while also benefiting from AWS Cloud storage capabilities. They plan to implement a solution that provides low-latency access to frequently used files while backing up data to AWS.
>
> Which AWS Storage Gateway configuration should they choose?
>
> A: Implement Storage Gateway in Cached Volume mode to keep frequently accessed data local while storing the complete dataset in Amazon S3.

---

> Q: AnyCompany Telecommunications is concerned about potential downtime after experiencing an outage last quarter. They want to implement a disaster recovery solution for their on-premises server fleet but have limited IT staff. The CEO is particularly concerned about maintaining exact replicas of production servers and minimizing recovery time.
>
> What is a key benefit of using AWS Elastic Disaster Recovery in this scenario?
>
> A: Continuous block-level replication with frequent backup intervals, providing near-instant recovery of servers at the target AWS Region

---

ASSESSMENT

> Q: What is the primary function of Amazon S3 storage classes?
>
> A: To provide different storage options optimized for different use cases and access patterns

> Q: Which statement BEST describes Amazon S3?
>
> A: A scalable object storage service that is used to store and retrieve any amount of data from anywhere on the web.

> Q: AnyCompany Manufacturing maintains a large amount of engineering drawings and design files that their teams need to access daily from their on-premises applications. They want to gradually migrate these files to AWS to reduce their local storage costs while maintaining low-latency access for frequently used files.
>
> The solution needs to meet the following criteria:
>
> - Integrate with existing file-based workflows.
> - Provide a seamless path to cloud storage without disrupting current operations.
> - Maintain local, low-latency access to frequently used files.
>
> Which AWS storage service should they use based on these requirements?
>
> A: AWS Storage Gateway – File Gateway

> Q: AnyCompany Software is deploying a critical production application on Amazon EC2 instances with several Amazon Elastic Block Store (Amazon EBS) volumes containing application code and customer data. The team is looking for an AWS service they can use to back up the data for their application.
>
> The solution needs to meet the following criteria:
>
> - Create regular data backups.
> - Create duplicate environments for testing.
> - Create a disaster recovery strategy.
> - Create full or incremental backups without impacting application performance.
> - Provide cost-effective for long-term storage.
>
> Which AWS service or feature would BEST meet the requirements in the scenario?
>
> A: EBS snapshots

> Q: AnyCompany AI is developing a machine learning application that requires extremely fast data processing for temporary model training datasets. The data is generated during training sessions and stored separately in persistent storage. The team is trying to determine the best storage solution to use alongside their application.
>
> The solution needs to meet the following criteria:
> - Highest possible I/O performance
> - Directly attached to their Amazon EC2 instances
> - Temporary storage – data does not persist when instances are stopped or terminated
>
> Which AWS service BEST meets the temporary storage needs described in this scenario?
>
> A: Amazon EC2 instance store

> Q: Which statement BEST describes Amazon Elastic Block Store (Amazon EBS)?
>
> A: A block-level storage service that provides persistent storage volumes for Amazon EC2 instances

> Q: Which statement BEST describes Amazon Elastic File System (Amazon EFS)?
>
> A: A fully managed, elastic file system that scales automatically as files are added and removed

> Q: What is a key characteristic of Amazon S3 storage classes pricing?
>
> A: Pricing varies based on storage costs, retrieval fees, and minimum storage durations.

> Q: AnyCompany Technology needs to implement a centralized storage solution for their development team that allows multiple Amazon EC2 instances to access the same file system simultaneously.
>
> The solution needs to meet the following criteria:
> - Provide a fully managed service.
> - Automatically scale.
> - Eliminate the need for capacity planning.
> - Support Linux-based applications with standard file system interfaces.
> - Maintain consistent low-latency access across development environments.
> - Provide high durability without requiring complex replication setups.
>
> Which AWS storage service is BEST suited for this scenario?
>
> A: Amazon Elastic File System (Amazon EFS)

> Q: AnyCompany Commerce has recently migrated its main application to an Amazon EC2 instance in AWS. As their customer base expands, they are exploring storage solutions that can grow dynamically with the application's data needs.
>
> The solution needs to meet the following criteria:
> - Have persistent block storage that provides consistent low-latency performance.
> - Be able to be attached to and detached from the EC2 instance as needed.
> - Independently resize storage capacity without disrupting the instance.
> - Create point-in-time backups to protect critical customer and inventory data.
>
> Which AWS storage service would BEST meet the requirements in the scenario?
>
> A:  Amazon Elastic Block Store (Amazon EBS)

> Q: Which statement BEST describes AWS Elastic Disaster Recovery?
>
> A: A service that minimizes downtime and data loss by providing fast, reliable recovery of on-premises and cloud-based applications using affordable storage, minimal compute, and point-in-time recovery

> Q: Which statement BEST describes AWS Storage Gateway?
>
> A: A hybrid cloud storage solution that provides on-premises applications with access to virtually unlimited cloud storage

> Q: Which statement BEST describes Amazon FSx?
>
> A: A fully managed service that provides cost-effective, scalable file storage built on widely used file systems

> Q: AnyCompany Marketing needs a storage solution that they can use to distribute large collections of high-resolution images, videos, and design files for their clients' campaigns. Some assets are accessed frequently, whereas others are archived for occasional reference.
>
> The solution needs to meet the following criteria:
> - Unlimited storage capacity
> - High durability
> - Easy file sharing through URLs
> - Ability to organize assets by client and project
> - Cost-efficient storage options
> - Security controls to prevent unauthorized access for specific assets
>
> Which AWS service is BEST suited for the storage needs described in this scenario?
>
> A: Amazon S3

> Q: AnyCompany Marketing needs to migrate their existing file shares to AWS to support their design teams who work with large creative files. They need help choosing a storage solution that can facilitate this migration.
> The solution needs to meet the following requirements:
> - Provide a fully managed service.
> - Seamlessly integrate with Windows applications.
> - Support SMB protocol.
> - Offer Active Directory integration for user authentication.
> - Support data deduplication to optimize storage costs.
> - Provide consistent sub-millisecond latencies.
> - Provide high availability.
>
> Which AWS storage service BEST meets the requirements described in the scenario?
>
> A: Amazon FSx for Windows File Server


---


## QUIZ Module 7 - Databases

> Q: AnyCompany Logistics is growing and expanding their online platform. The development team must choose between two database options. They can host their own database on an Amazon EC2 instance or use AWS's fully managed database service. The company wants to reduce IT maintenance tasks so their staff can focus more on development work.
>
> Which option should they choose?
>
> A: Choose a managed database service, because the team wants to focus on developing new features rather than database administration tasks.

---

> Q: AnyCompany Retail wants to migrate its product database to the AWS Coud to reduce operational overhead. Their existing database contains critical inventory and pricing information that requires continuous operation with minimal downtime. Management is exploring Amazon RDS as a way to reduce the number of IT resources.
>
> Which feature of Amazon RDS addresses the database requirements described in this scenario?
>
> A: Multi-AZ deployments

> Q: AnyCompany Financial is experiencing slow response times with their current MySQL database during peak transaction periods. It processes over 100,000 transactions per hour and requires high throughput for customer satisfaction. The CTO is looking at Amazon Aurora as a way to significantly improve database performance.
>
> Which Aurora feature BEST addresses this scenario?
>
> A: Aurora provides a high-performance, highly available storage architecture that offers up to five times the throughput of standard MySQL.

---

> Q: A staffing resource company is building an application that must store employee information with unpredictable traffic patterns. Their application requires consistent performance at all times, and the development team wants to focus on features rather than database management tasks.
>
> Which Amazon DynamoDB capability BEST addresses the needs for this workload?
>
> A: Auto scaling with provisioned capacity

---

> Q: Which problem does Amazon ElastiCache solve?
>
> A: Performance bottlenecks due to high latency and throughput constraints

> Q: What is the main problem that can be solved by implementing AWS Backup?
>
> A: Fragmented backup approaches across different AWS services

> Q: What is a primary feature of Amazon DocumentDB?
>
> A: MongoDB compatibility

> Q: What is a benefit of using Amazon Neptune?
>
> A: Low-latency queries on highly connected data

ASSESSMENT

> Q: What is a practical use case for Amazon DocumentDB (with MongoDB compatibility)?
>
> A: Storing and managing a large product catalog for an ecommerce application

> Q: What is the primary way that NoSQL databases like Amazon DynamoDB differ from relational databases?
>
> A: NoSQL databases use flexible schema designs rather than the rigid table structures of relational databases.

> Q: Which statement describes the responsibilities of customers using fully managed AWS database services?
>
> A: Customers are responsible for designing data structures and managing access controls.

> Q: Which explanation BEST describes Amazon RDS?
>
> A: A fully managed service that helps set up, operate, and scale relational databases in the cloud

> Q: What is a feature of AWS Backup?
>
> A: AWS Backup provides centralized backup policies and monitoring across multiple AWS accounts and Regions.

> Q: What is a possible use case for Amazon Aurora?
>
> A: Replacing high-cost commercial database engines with a more cost-effective solution that still provides enterprise-level performance and reliability ????

> Q: Which problem does AWS Database Migration Service (AWS DMS) solve?
>
> A: Minimizing application downtime during database migrations

> Q: Which definition BEST describes in-memory caching?
>
> A: A cloud-based service that stores data in memory for fast access, improving application performance and scalability while reducing database load

> Q: Which definition BEST describes in-memory caching?
>
> A: A cloud-based service that stores data in memory for fast access, improving application performance and scalability while reducing database load

> Q: Which option describes a scenario where an unmanaged solution like a database installed directly onto an Amazon EC2 instance would be preferable to using a fully managed AWS database service?
>
> A: A developer needs full control over the database and access to its underlying operating system, database installation, and configuration.

> Q: What is a primary benefit of using Amazon ElastiCache?
>
> A: Improved application performance through in-memory caching

> Q: What is a practical use of Amazon Neptune?
>
> A: Managing and querying highly connected datasets efficiently

> Q: Which statement BEST describes Amazon DynamoDB?
>
> A: DynamoDB is a fully managed NoSQL key-value and document database that provides fast, predictable performance with seamless scalability.


---

## QUIZ Module 8 - AI/ML and Data Analytics

> Q: Machine learning (ML) is a type of AI for training machines to perform complex tasks without explicit instructions. This training process involves finding patterns in vast amounts of historical data.
>
> What is produced as a result of the ML training process?
>
> A: An ML model that can make predictions or decisions


> Q: The owner of a car dealership wants to determine why her service department has lost business over the past year. She wants to analyze a large number of documented customer comments to better understand customer sentiment.
>
> Which AWS service would work well for this use case?
>
> A: Amazon Comprehend

> Q: A healthcare company wants to add a conversational interface to its customer support application using a ready-made solution.
>
> Which AWS service could they choose?
>
> A: Amazon Lex

> Q: An instructional designer is developing a new course on customer service skills. He wants to include several simulated calls to reinforce the learning. Because he doesn't have access to a recording studio, he needs a quick way to convert his scripts to speech.
>
> Which service would work well for this use case?
>
> A: Amazon Polly

> Q: A small tech company wants to develop their own customized machine learning (ML) model without managing the underlying infrastructure. The company is looking for a solution that both their data scientists and business analysts can use.
>
> Which AWS service should they choose?
>
> A: Amazon SageMaker AI

> Q: A team of machine learning (ML) engineers is developing a new ML model for a highly specialized application. They need complete control over the ML training process. So, they are developing their own custom solution using the PyTorch ML framework.
>
> What is an ML framework?
>
> A: A software library with pre-built, optimized components

> Q: Generative AI is a type of deep learning powered by extremely large ML models that are pre-trained on vast collections of data.
>
> What are these models called?
>
> A: Foundation models

---

> Q: A large advertising agency wants to quickly integrate a new content generation feature into its existing enterprise-wide design application. The new feature needs to be able to generate both text and images. The agency doesn't want to manage any new infrastructure.
>
> Which service would work best for this use case?
>
> A: Amazon Bedrock

> Q: A software development company is working on a new product with a very tight deadline. The company needs a way to develop code faster without sacrificing reliability or security.
>
> Which service could best help this company meet its deadline?
>
> A: Amazon Q Developer

---

> Q: Data pipelines are automated assembly lines used to make the ETL process efficient and repeatable.
>
> What does ETL stand for?
>
> A: Extract, transform, load

> Q: In the field of data analytics, analysts transform raw historical data into something useful.
>
> What are these analysts working to uncover with this transformed data?
>
> A: Valuable insights and trends

---

> Q: A data analytics team is creating an automated data pipeline on AWS.
>
> Which AWS services could they choose for data ingestion? (Select TWO.)
>
> A: Amazon Kinesis Data Streams / Amazon Data Firehouse

> Q: The data analytics team must ingest vast amounts of unstructured data into its pipeline.
>
> Which AWS service is the BEST choice for storing this data?
>
> A: Amazon S3

> Q: Which AWS service is BEST suited for data processing in a data pipeline?
>
> A: AWS Glue

> Q: Which AWS services could the data analytics team choose for data visualization? (Select TWO.)
>
> A: Amazon QuickSight / Amazon OpenSearch

ASSESSMENT

> Q: The extract, transform, load (ETL) process is often used to provide clean and accessible data in a format that is usable by analytics tools and AI algorithms.
>
> How does a data pipeline improve this process?
>
> A: Data pipelines make the ETL process more efficient and repeatable.

> Q: A large healthcare organization wants to improve employee productivity. The company is searching for a pre-built generative AI assistant that can answer questions, help solve problems, and take actions using the data and expertise found in its information repositories.
>
> Which AWS service would work well for this use case?
>
> A: Amazon Q Business

> Q: Amazon Bedrock is a fully managed service that was specifically designed for working with large foundation models (FMs) and building generative AI applications.
>
> What does the service provide to access FMs from Amazon and leading AI startups?
>
> A: A single API ??????

> Q: Generative AI is a type of deep learning powered by extremely large machine learning (ML) models known as foundation models (FMs).
>
> What are characteristics of FMs? (Select TWO.)
>
> A: FMs can be adapted to perform multiple tasks. / FMs are pre-trained on vast collections of data.

> Q: Which AWS service can be used to build, train, and deploy a customized machine learning (ML) model without worrying about the underlying infrastructure?
>
> A: Amazon SageMaker AI

> Q: Both classical programming and machine learning can be used to train computers to perform tasks.
>
> What is the main difference between the two approaches?
>
> A: Classical programming creates explicit rules for the computer to follow. In machine learning, computers make predictions using patterns learned from historical data.

> Q: An e-commerce company wants to add a product recommendation engine to its online application to increase sales. The development team wants the recommendations to be relevant for each individual customer.
>
> Which pre-built AWS AI service would work well for this use case?
>
> A: Amazon Personalize

> Q: A financial services company is developing an application to analyze real-time stock data so its team of analysts can make immediate trading decisions. The company needs to ingest real-time stock market data without worrying about servers or scaling capacity.
>
> Which AWS service would meet their needs?
>
> A: Amazon Kinesis Data Streams

> Q: A small development team is looking to add a feature to its application that converts text to speech.
>
> Which pre-built AWS AI service can be used for this task?
>
> A: Amazon Polly

> Q: Data can come from many different sources. To provide insights, the data must be consolidated in a single location. There are two storage options for this. Data lakes store vast amounts of raw data, and data warehouses are optimized for business intelligence.
>
> Which AWS services are typically used as a data lake and data warehouse?
>
> A: Amazon S3 is a popular choice for data lakes, whereas Amazon Redshift is a data warehouse service.

---

## QUIZ Module 9 - Security

> Q: After logging in to their online banking profile with their username and password, a customer attempts to transfer $10,000 from their savings to their checking account. The system checks if the customer has sufficient privileges to make transfers of this amount before proceeding.
>
> Which type of system check is this an example of?
>
> A: Authorization

> Q: A healthcare company is preparing to deploy a web application on Amazon EC2 instances that will process sensitive patient data. The application will use Amazon RDS for database storage and Amazon S3 for file storage. The company's security team is discussing security responsibilities for the deployment.
>
> What is the customer's security responsibility in this scenario?
>
> A:  Protecting sensitive patient data stored in Amazon S3 and Amazon RDS

---

> Q: An administrator who creates an AWS account is provided with the root user credentials. To secure this highly privileged account, they should immediately set a strong password and enable multi-factor authentication (MFA).
>
> What does MFA require users to do?
>
> A: Provide two or more verification methods to gain access.

> Q: AWS Identity and Access Management (IAM) provides users, groups, roles, and policies so you can configure access based on your company’s specific operational and security needs.
>
> Which of these is specifically designed to provide temporary access to permissions?
>
> A: IAM roles

> Q:A financial services company wants to give its accountants access to a particular Amazon S3 bucket.
>
> Which of these IAM controls is used to define this access?
>
> A: IAM policy

---

> Q: A software development team needs to centrally manage its database credentials and API keys on AWS.
>
> Which of these services should the team choose?
>
> A: AWS Secrets Manager

> Q: In a denial of service (DoS) attack, an attacker floods a web application with excessive network traffic. Legitimate customer requests are denied if the web application becomes overloaded and can no longer respond.
>
> How is a distributed denial of service (DDoS) attack different?
>
> A: A DDoS attack uses multiple compromised computers and devices to launch the attack.

> Q: An online boutique has recently suffered a series of targeted distributed denial of service (DDoS) attacks. The owner wants to enhance the security of the boutique's web application using AWS infrastructure.
>
> Which components can the boutique use to protect the web application on AWS from DDoS attacks? (Select TWO.)
>
> A: Security groups / Elastic Load Balancing (ELB)

--- 

> Q: Which processes involve locking and unlocking data with a special key so only authorized users can access it?
>
> A: Encryption and decryption

> Q: A tax preparation company needs to secure sensitive customer data moving from its database to its web application on AWS.
>
> Which of these services can help them secure the data in transit?
>
> A: AWS Certificate Manager (ACM)

> Q: A security team at a legal firm has detected a threat to their AWS environment. To investigate the root cause over time, they need interactive visualizations of security data.
>
> Which AWS service is the BEST choice for this investigation?
>
> A: Amazon Detective

> Q: A local government agency needs to prepare for an upcoming compliance audit. The agency needs to automatically aggregate security findings from multiple AWS services into one comprehensive view.
>
> Which of these services should the agency choose?
>
> A: AWS Security Hub

ASSESSMENT

> Q: With AWS Identity and Access Management (IAM) all actions are denied by default. When granting permissions, access should be provided only on a need-to-have basis.
>
> What is this concept called?
>
> A: Principle of least privilege

> Q: What is the responsibility of AWS under the AWS shared responsibility model?
>
> A: Managing physical security of data centers

> Q: A security team for a large ecommerce company needs a centralized way to create and manage the encryption keys that protect its data on AWS.
>
> Which of these services is the BEST fit for this team?
>
> A: AWS Key Management Service (AWS KMS)

> Q: A small financial services company recently moved its online resources to AWS. The security team was concerned about protection from common, frequently occurring types of distributed denial of service (DDoS) attacks.
>
> Which AWS service automatically protects customers at no cost from DDoS attacks?
>
> A: AWS Shield

> Q: An employee wants to check their company’s online employee portal to see how many vacation hours they have accrued. Before accessing their personal records, they enter their username and password to log in to the site.
>
> What happens during this login process?
>
> A: Authentication

> Q: A security team for a large software development company needs to check multiple applications for security vulnerabilities and deviations from security best practices. The applications are running on Amazon EC2, AWS Lambda, and in containers.
>
> Which AWS service should they choose for the security assessments?
>
> A: Amazon Inspector

> Q: A technology company is moving some of its resources to AWS. The company wants to provide single sign-on access for its employees on AWS using its existing identity source.
>
> Which service can help the company accomplish this?
>
> A: AWS IAM Identity Center

> Q: A large marketing firm has a standard set of permissions used to grant designers access to certain Amazon S3 buckets. The firm added a new S3 bucket that all designers need to access.
>
> Which AWS Identity and Access Management (IAM) control can the firm use to assign permissions that will be inherited by all of its designers?
>
> A: IAM group

> Q: All AWS accounts are given an AWS account root user. The root user is the account owner and has full permissions to perform any actions.
>
> What are some ways to protect this powerful account? (Select TWO.)
>
> A: Associate a strong password with the account. /  Turn on multi-factor authentication (MFA).

> Q: Protecting sensitive customer data is a vital component of maintaining customer trust. This involves encrypting data at rest and in transit.
>
> What is used to encrypt data in transit?
>
> A: SSL/TLS certificates


---

## QUIZ Module 10 - Monitoring, Compliance, and the Governance in the AWS Cloud

> Q: An ecommerce company is hosting their customer application on multiple Amazon EC2 instances. The application experiences fluctuating traffic and occasional performance issues that are impacting the customer experience.
>
> How can Amazon CloudWatch help the customer? (Select THREE.)
>
> A:
>   - CloudWatch dashboards can be customized to visualize the metrics, alarms, and data in a consolidated view.
>   - CloudWatch alarms can be set up to alert when the Amazon EC2 utilization is too high for an extended period and automate more EC2 instances being created to share the load.
>   - CloudWatch logs can collect data on the EC2 instances and application logs. The logs can gain insights on performance issues or application errors.

---

> Q: A company wants to store the files that contain API activities for an AWS account in an Amazon S3 bucket. They want to retain these files for auditing and compliance.
>
> Which solution and feature would provide this capability?
>
> A: AWS CloudTrail logs

---

> Q: Which tasks can you complete in AWS Artifact? (Select TWO.)
>
> A:
>  - Access AWS compliance reports on demand.
>  - Review, accept, and manage agreements with AWS.

> Q: An enterprise customer with a large team of developers needs a way to ensure specific configuration guidelines for the developers when creating AWS resources. They want to assess and audit the AWS resources to make sure that the team is using the most cost-effective approved list of Amazon EC2 instances.
>
> Which AWS service would best fit the customer's need?
>
> A: AWS Config

---

> Q: You are configuring service control policies (SCPs) in AWS Organizations.
>
> Which identities and resources can SCPs be applied to? (Select TWO.)
>
> A:
> - An individual member account
> - An organizational unit (OU)

---

> Q: A government customer needs to set up and govern a secure, compliant, multi-account AWS environment. They want to make sure that employees comply with their approved requirements when creating new AWS accounts.
>
> Which AWS service would best fit the customer's need?
>
> A: AWS Control Tower

---

> Q: An enterprise customer with a multi-Region AWS network is looking for ways to continuously evaluate and reduce costs while making sure that everything is secure and performing efficiently. They are also interested in learning AWS best practices to apply to their operations.
>
> Which solution would BEST meet their needs?
>
> A: AWS Trusted Advisor

ASSESSMENT

> Q: A financial company is looking for a solution to govern a curated set of AWS resources for their employees. When the employees need to select and start up a new AWS resource, they want to provide a self-service way to create, share, and deploy the AWS resources.
>
> Which AWS service would best meet their needs?
>
> A: AWS Service Catalog
>
> _With Service Catalog, you can create, share, and organize from a curated catalog of AWS resources. You can deploy baseline networking resources and security tools for new AWS accounts so that you can govern consistently._

> Q: A customer is using AWS Organizations to centrally manage their company's accounts for billing to optimize and organize costs. They want to set up rules or restrictions on the AWS services, resources, and individual API actions that the users can access.
>
> Which feature would meet their needs?
>
> A: A service control policy (SCP)
>
> _An SCP is a policy that lets you place restrictions on the AWS services, resources, and individual API actions that users and roles in each account can access. SCPs can be applied to either OUs or individual member accounts._

> Q: Which AWS service provides a no-cost, on-demand access to AWS security and compliance reports and select online agreements?
>
> A: AWS Artifact
>
> _AWS Artifact is a self-service portal that provides on-demand access to AWS security and compliance documentation, including reports._

> Q: A sportswear company is hosting their application on Amazon EC2 instances. They want to collect metrics on their EC2 instances, and they would like notifications when utilization passes thresholds. They also want to have an action configured to automate scaling up the number of EC2 instances when utilization surpasses their threshold.
>
> Which AWS service would best meet their needs?
>
> A: Amazon CloudWatch
>
> _CloudWatch can collect the metrics on the EC2 instances, provide insights using dashboards, set alarms on thresholds, and automate the additional EC2 instances._

> Q: A research customer with a large team of developers needs a way to ensure specific configuration guidelines for the developers when creating AWS resources. They want a way to assess and audit the AWS resources to ensure that the team is using the most cost-effective approved list of compute resources.
>
> Which solution or feature would meet their needs?
>
> A: AWS Config
>
> _AWS Config is the best choice because it will assess, audit, and evaluate the configurations of the developer's AWS resources._

> Q: An enterprise customer has grown rapidly and is struggling to manage billing of their AWS resources and accounts. Every employee has created independent accounts with no centralized management or hierarchical groupings of accounts. The customer wants to roll up billing and centralize management into organizational units.
>
> Which AWS service would best meet this customer's need?
>
> A: AWS Organizations
>
> _With Organizations, you can centrally manage your environment as you scale your AWS resources. It can be used to centralize management, consolidate billing, and implement hierarchical groupings of accounts._

> Q: A financial company with a hybrid cloud solution wants to track changes made to their AWS resources both in the cloud and on premises. Specifically, they want to know who did what, and when.
>
> Which AWS service would best meet their needs?
>
> A: AWS CloudTrail
>
> _CloudTrail is an AWS service that uses APIs to track who did what, when the action occurred, and on which AWS services and resources._

> Q: Which AWS service provides continuous evaluation and checks of your AWS resources, and provides suggestions to optimize costs, performance, security, and resilience?
>
> A: AWS Trusted Advisor
>
> _Trusted Advisor helps you optimize costs, increase performance, improve security and resilience, and operate at scale in the cloud._

> Q: Where can customers go to find resources on AWS compliance—for example, information on customer compliance stories, answers to key compliance questions, and an auditing security checklist?
>
> A: Customer Compliance Center
>
> _The Customer Compliance Center provides resources to help you learn more about AWS compliance. You can read customer compliance stories to discover how companies in regulated industries have solved various compliance, governance, and audit challenges._

> Q: What is the purpose of an AWS Control Tower landing zone?
>
> A: It is the enterprise-wide container that holds all your organizational units (OUs), accounts, users, and resources that you want to regulate for compliance.
>
> _A landing zone is a well-architected multi-account environment that is based on security and compliance best practices. It is the container where you hold all the resources that you want to regulate for compliance._

> Q: A customer is moving from on premises to the cloud and has decided to use the Bring Your Own License model (BYOL) approach for cost savings. They are concerned about managing the licenses, want a way to reduce the risk of noncompliance, and want to enforce license usage limits.
>
> Which solution would best meet their needs?
>
> A: AWS License Manager
>
> _License Manager helps reduce the risk of noncompliance by enforcing license usage limits, blocking new launches, and using other controls._


---

## QUIZ Module 11 - Pricing and Support

> Q: You work as a cloud engineer for a health care company. The chief technology officer wants to store patient records in the cloud. They ask you about the driving factors of cost.
>
> Which answer BEST describes the key driving factors of cost for the AWS Cloud?
>
> A: Although pricing factors into multiple service categories, the primary driving factors of cost are compute, storage, and data transfer.

> Q: A government agency is getting started with managing their AWS Cloud costs. They want to set up notifications to alert them when costs exceed a certain threshold for any given month.
>
> Which AWS service would they use to achieve this task?
>
> A: AWS Budgets

---

> Q: A mid-sized company is trying to decide the level of AWS Support that best suits their needs. The company has the following requirements:
> - Timely assistance, but not necessarily 24/7 support
> - Basic AWS Trusted Advisor security checks
> - General guidance on best practices
> - Support for incident response and troubleshooting within 12–24 hours
>
> Which AWS Support Plan should the company choose based on these requirements?
>
> A: Developer Support

> Q: You are a new cloud solutions architect at a growing tech company. Your manager has asked you to explore the AWS Marketplace to find solutions that can help improve your company's operational efficiency and reduce costs.
>
> Based on what you've learned, which options are available on the AWS Marketplace? (Select TWO.)
>
> A:
>   - Software as a service (SaaS) applications
>   - Datasets and analytics tools

---

ASSESSMENT

> Q: Which option BEST describes a key benefit of being an AWS Partner?
>
> A: AWS Partner Funding benefits
>
> _One of the key benefits of being an AWS Partner is access to various funding benefits. These can include financial incentives, marketing support, and go-to-market funding that help partners build, market, and sell their solutions on AWS._

> Q: An EdTech company is considering moving their education application to the cloud. The company's chief financial officer (CFO) wants to understand how AWS services are priced and which factors will drive their cost.
>
> Although pricing varies based on several factors, which options are the fundamental drivers of cost with AWS? (Select THREE.)
>
> A:
>   - Outbound data transfer
>   - Storage
>   - Compute
>
> _The cost of an AWS service or category of services can be impacted by several factors. However, the primary driving factors of cost are compute, storage, and outbound data transfer._

> Q: A large enterprise wants to find compliance-ready software solutions to make sure they meet industry regulations. They are exploring AWS services to help with this, and they want to implement the solution as quickly as possible.
>
> What option is the BEST fit for this enterprise and their requirements?
>
> A: Find compliance-ready solutions in the AWS Marketplace.
>
> _AWS Marketplace offers a variety of software solutions such as compliance-ready software. This enterprise can use the AWS Marketplace to quickly find and implement a solution that meets their specific needs._

> Q: A global finance company currently has their information technology (IT) resources on-premises and is evaluating the AWS Cloud. The company is used to fixed capital expenditures and wants to understand how they would pay by moving to the AWS Cloud.
>
> Which choices BEST describe how customers pay for AWS? (Select THREE.)
>
> A:
>   - Save when you commit
>   - Pay as you go
>   - Pay less by using more
>
> _When it comes to AWS pricing, customers pay as they go and can save when they commit to a specific amount of usage for a certain period of time. They can also get volume-based discounts as their usage increases._

> Q: You are part of a team that wants to monitor and manage costs of multiple AWS accounts across different departments within your organization.
>
> Which AWS service can you use to effectively manage and consolidate billing information for these accounts?
>
> A: AWS Organizations

> Q: You are the chief technology officer of a large enterprise with mission-critical applications running on AWS. Your organization requires the highest level of support, including response times of 15 minutes or less when mission-critical systems are down.
>
> Which AWS support plan should you choose?
>
> A: Enterprise Support
>
> _Enterprise Support is designed for large enterprises with mission-critical applications. It offers the highest level of support, including rapid response times, proactive monitoring, and access to a wide range of AWS services and features. Additionally, it provides guidance from AWS experts to help ensure optimal performance and security._

> Q: In addition to AWS Support Plans and other technical assistance options, AWS also provides access to self-support resources.
>
> Which options do AWS customers have available as self-support resources? (Select THREE.)
>
> A:
>   - SDK guides
>   - AWS Documentation, such as user guider for AWS services
>   - AWS Blog

> Q: An online retail company is interested in moving forward with the migration of an application, but they would like to estimate costs before diving in.
>
> Which tool or service can they use to estimate the cost of the specific AWS services and configurations that they need?
>
> A: AWS Pricing Calculator is a web-based tool that the company can use to configure cost estimates for their unique business needs.

> Q: You are the technical lead for a mid-sized e-commerce company and are evaluating various support options for your AWS infrastructure. Your current challenges include optimizing database performance and incident response planning. You are also seeking technical consulting on best practices for security.
>
> Outside of standard AWS Support Plans, which support option is the BEST choice for getting advice on best practices for security and for conducting a security audit of your AWS environment?
>
> A: AWS Professional Services
>
> _AWS Professional Services offers deep technical expertise and can assist with security audits, best practices, and strategic guidance tailored to specific needs._

> Q: Which option BEST describes the role of the AWS Partner Network (APN)?
>
> A: Helping businesses build, market, and sell solutions based in AWS
>
> _The APN helps AWS Partners build, market, and sell solutions based in AWS by providing them with technical, marketing, and go-to-market support._


---

## QUIZ Module 12 - Migrating to the AWS Cloud


> Q: Which perspective of the AWS Cloud Adoption Framework (AWS CAF) includes principles and patterns for implementing new solutions in the cloud and migrating on-premises workloads to the new platform in the cloud? It uses a variety of architectural models to understand and communicate the structure of IT systems.
>
> A: Platform perspective

---

> Q: Which migration strategy involves moving to a different product?
>
> A: Repurchasing

---

> Q: A customer is getting started on their migration and is not sure how to build a business case to justify their move.
>
> Which solution would BEST meet the requirements?
>
> A: Migration Evaluator

> Q: A customer is looking for a tool to help centralize the view of all their migration tasks and help track their migration.
>
> Which solution would BEST meet the requirements?
>
> A: AWS Migration Hub

---

> Q: An enterprise customer wants to migrate their on-premises databases to the AWS Cloud. They are interested in changing their current commercial database to an open source database to reduce licensing costs. They need help converting all the database objects to the new database type.
>
> Which AWS service would BEST fit the customer's need?
>
> A: AWS Schema Conversion Tool (AWS SCT)

---

> Q:  A healthcare company is migrating large amounts of data between their on-premises storage in Amazon S3. They want to automate the process and be able to schedule the migration to off-peak times and be able to check on progress and task reporting.
>
> Which service would best meet their need to transfer the data?
>
> A: AWS DataSync

ASSESSMENT

> Q: What are the seven migration strategies that are commonly used when customers migrate to the AWS Cloud?
>
> A: Relocate, Rehost, Replatform, Refactor, Repurchase, Retain, and Retire

> Q: What is the primary function of the AWS Cloud Adoption Framework (AWS CAF)?
>
> A: It provides tools to help accelerate the migration journey, organize resources, and align management during the transition.

> Q: An environmental agency is migrating their applications to the AWS Cloud. During the migration they also want to look for ways to modernize and reduce costs of their applications.
>
> Which migration service would BEST meet their needs?
>
> A: AWS Application Migration Service

> Q: The migration team wants to make sure the organization considers a company-wide change management strategy for successful cloud adoption. Which Cloud Adoption Framework (CAF) perspective would they use?
>
> A: People

> Q: An engineering company is migrating large amounts of proprietary intellectual property design files from their on-premises data center to the AWS Cloud. They want a service that has fully managed support for secure file transfers with several different protocols, like Secure File Transfer Protocol (SFTP) and File Transfer Protocol Secure (FTPS)
>
> Which online migration solution would meet their needs?
>
> A: AWS Transfer Family

> Q: A retail company is just getting starting with their migration to the AWS Cloud. They need help building a business case to secure funding from their chief financial officer (CFO) and stakeholders.
>
> Which migration service would BEST meet their needs?
>
> A: Migration Evaluator

> Q: A media company is in the migrate and modernize phase of their migration and wants a centralized location to view their migration tasks and progress.
>
> Which migration service would BEST meet their needs?
>
> A: AWS Migration Hub

> Q: During their upcoming migration, the database administrator would like to move from their current database to an AWS managed database to offload some of the database administration. They would also like to use a tool to plan, assess, convert, and migrate the database.
>
> Which migration solution would BEST meet their needs?
>
> A: AWS Database Migration Service (AWS DMS)
>
> _Database Migration Service makes it possible to quickly and securely migrate databases and data replication to the AWS Cloud. It provides a way to plan, assess, convert, and migrate databases even with data warehouses in one central tool and can be used when converting databases._

> Q: A credit card company is migrating large amounts of sensitive data from their on-premises storage to the AWS Cloud. They want to automate the process and schedule the migration during off peak times. They also want to be able to check on progress and task reporting. They do not have a dedicated private connection between their data center and the AWS Cloud.
>
> Which online migration solution would meet their needs?
>
> A: AWS DataSync

---

## QUIZ Module 13 - Well architected Solutions

> Q: A development team for a small marketing company needs a debugging and performance analysis tool to visualize their online application’s behavior. The application is hosted on AWS.
>
> Which AWS service should this team choose?
>
> A: AWS X-Ray
>
> _X-Ray provides visualization tools specifically designed for debugging and performance analysis of applications._

> Q: A large automotive company wants to use the power of AI in its customer service center. They need a solution that includes call routing, recording, and analytics.
>
> Which AWS service can provide these capabilities?
>
> A: Amazon Connect
>
> _Amazon Connect is an AI-powered contact center solution that offers call routing, recording, and analytics capabilities._

> Q: An IT department needs to provide employees access to several software-as-a-service (SaaS) online applications.
>
> Which AWS service can provide this access?
>
> A: Amazon AppStream 2.0
>
> _AppStream 2.0 delivers desktop applications to users through web browsers, enabling secure SaaS application access for employees._

> Q: Which options are Internet of Things (IoT) solutions? (Select TWO.)
>
> A:
>   - A wearable device that tracks steps per day on a smartphone
>   - A Wi-Fi enabled plug that can be used to turn of lights remotely
>
> _The wearable device that tracks steps on a smartphone and the Wi-Fi enabled plug that can be used to turn off lights remotely are both examples of IoT solutions. Although these other options are digital solutions, they do not involve physical devices that communicate with networked applications._

---

> Q: A development team is releasing frequent updates to an application hosted on AWS. Right now, each deployment requires manual steps that often result in downtime or inconsistent environments.
>
> What AWS practice from the Well-Architected Framework could help in this situation?
>
> A: Automate deployments through a continuous integration and continuous delivery pipeline (Operational Excellence).

> Q: What is the purpose of the AWS Well-Architected Tool (AWS WA Tool)?
>
> A: To assess and improve cloud workloads based on six key architectural pillars

---

ASSESSMENT

> Q: The owner of a large hardware company wants to automate and optimize the company’s marketing emails to enhance customer engagement.
>
> Which AWS service would work well for this use case?
>
> A: Amazon Simple Email Service (Amazon SES)

> Q: A startup is hosting a critical web application on a single Amazon EC2 instance in one Availability Zone. After a brief outage, they decide to reevaluate their architecture.
>
> What practices from the AWS Well-Architected Framework could improve this situation?
>
> A: Deploy instances across multiple Availability Zones for fault tolerance (Reliability).

> Q: A small technology startup needs to provide its remote workforce with secure access to their work environment. The employees must be able to accomplish the same tasks as if they were on a physical office computer.
>
> Which AWS service can they use to provide this remote access?
>
> A: Amazon WorkSpaces

> Q: A developer is working on a full-stack application hosted on AWS. They are interested in streamlining the development process by quickly adding features like authentication and storage with minimal infrastructure management.
>
> Which AWS service would provide the best solution for the developer's needs?
>
> A: AWS Amplify

> Q: A company is using a large Amazon EC2 instance type for a low-traffic website, but monitoring shows CPU usage rarely exceeds 10 percent.
>
> What is a good next step?
>
> A: Rightsize the EC2 instance to a smaller type to match the actual workload.

> Q: A manufacturing company needs a way to monitor its assembly-line equipment for any performance issues.
>
> Which AWS service can help them build a monitoring solution for the equipment?
>
> A: AWS IoT Core
