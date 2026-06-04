# Module 2 - Compute in the cloud
- `Compute in the cloud` - Compute in the cloud means creating virtual machines with a cloud provider to run applications and tasks over the internet
- `Elastic Compute Cloud (EC2)` - Virtual Server/Machine in the AWS Cloud that provides on-demand, scalable computing capacity
- `EC2 Instances types`
    - General purpose - Balanced resources
    - Compute optimized - Compute intensive tasks
    - Memory optimized - Provide fast performance for memory-heavy workloads
    - Accelerated computing - Uses HW acceleators to efficiently handle tasks
    - Storage optimized - Designed for workloads that require high performance for lacally stored data
- `AWS Management Console` - Web interface for managing AWS services
- `AWS Command Line Interface (CLI)` - Managing multiple AWS services directly from the command line.
- `AWS Software Development Kit (SDK)` - Simplifies integrating AWS services into your applications by providing APIs for various programming languages.
- `Amazon Machine Images (AMI)` - AMIs are pre-built VM that have the basic components for what is needed to start an instance.
    - It provides a consistent image to launch new instances.
    - With an _unmanaged_ service like EC2, you are responsible for configuring and managing security.
- `EC2 Pricing`
    - On-Demand Instances - Pay only for the compute capacity you consume with no upfront payment or long-term commitments required.
    - Reserved Instances - Get a saving of up to 75 percent by committing to a 1-year or 3-year term for predictable workloads using specific instance families and AWS Regions
    - Spot Instances - Bid on a spare compute capacity at up to 90 percent of the On-demand price, with the flexibility to be interrupted when AWS reclaims the instance
    - Savings Plans - Save up to 72 percent across a variety of instance types and services by commiting to a consistent usage level for 1 or 3 year.
    - Dedicated Hosts - Reserve an entire physical server for your exclusive use. This option offers full control and is ideal for workloads with strict security or licensing needs
    - Dedicated Instances - Pay for instances running on HW dedicated solely to your account. This option provides isolation from other AWS customers.
- `Cost optimization`
    - Saving Plans - Good for Predictable workloads
    - Capacity Reservation - Good for Critical workloads with strict capacity requirements
    - Reserved Instance flexibility - Good gor Steady-state workloads with predictable usage
- `Scalability` - Adding Resources
    - Scaling Up (Vertical) - Adding more power to existing machines
    - Scaling Out (Horizontal) - Adding more machines
- `Elasticity` - Abilitiy to automatically scale resources up or down in response to real-time demand
- `EC2 Auto Scaling` - automatically adjusts the number of EC2 instances based on changes in application demand, providing better availability. It offers two approaches.
    - Dynamic scaling adjusts in real time to fluctuations in demand.
    - Predictive scaling preemptively schedules the right number of instances based on anticipated demand.
- `Auto Scaling Group` - Configured with three key settings (**min, desired and max** capacity)
    -   - A load balancer serves as the single point of contact for all incoming web traffic to an Auto Scaling group.
- `Elastic Load Balancing (ELB)` - automatically distributes incoming application traffic across multiple resources, such as EC2 instances, to optimize performance and reliability.
    - Regional application
- `ELB Benefits`
    - Efficient traffic distribution - ELB evenly distributes traffic across EC2 instances, preventing overload on any single instance and optimizing resource utilization.
    - Automatic Scaling - ELB scales with traffic and automatically adjusts to changes in demand for a seamless operation as backend instances are added or removed.
    - Simplified management - ELB decouples front-end and backend tiers and reduces manual synchronization. It also handles maintenance, updates, and failover to ease operational overhead.
- `ELB Routing Methods`
    - Round Robin - Distributes traffic evenly across all available servers in a cyclic manner.
    - Least Connections - Routes traffic to the server with the fewest active connections, maintaining a balanced load.
    - Ip Hash - Uses the client’s IP address to consistently route traffic to the same server.
    - Least Response Time - Directs traffic to the server with the fastest response time, minimizing latency.
- `Monolitich Applications` - Applications consist of multiple components that work together to transmit data, fulfill requests, and keep the application running smoothly.
- `Microservices Applications` - Application components are loosely coupled. The communication between components remains intact, and the failure of a single component does not impact the entire system.
- `EventBridge` - A serverless service that helps connect different parts of an application using events, helping to build scalable, event-driven systems.
    - With EventBridge, you route events from sources like custom apps, AWS services, and third-party software to other applications.
- `Amazon Simple Queue Service (Amazon SQS)` - A message queuing service that facilitates reliable communication between software components.
    - It can send, store, and receive messages at any scale, making sure messages are not lost and that other services don't need to be available for processing
- `Payload` - Data contained within a message
- `SQS queues` - Where messages are placed until they are processed
- `Amazon Simple Notification Service (Amazon SNS)` - A publish-subscribe service that publishers use to send messages to subscribers through SNS topics.
- `SNS topic` - A channel for messages to be delivered

### Recap

In these lessons about compute, you learned how Amazon EC2 and cloud resources help scale applications. You gained knowledge of EC2 instance types, pricing options, and how to choose the best instance types for your unique business needs. You also became familiar with using AWS tools and services like Elastic Load Balancing, Amazon EC2 Auto Scaling, Amazon SQS, and Amazon SNS to manage traffic and communication.


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


## ASSESMENT


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