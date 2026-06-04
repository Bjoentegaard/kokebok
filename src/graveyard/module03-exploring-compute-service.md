# Module 3 - Exploring Compute Service
- `Unmanaged services` - (EX: EC2) AWS takes care of the underlying physical infrastructure, but you're responsible for setting up, securing, and maintaining the operating system, network configurations, and applications on your instances.
- `Managed services` - Managed services, on the other hand, reduce the amount of infrastructure you need to manage.
- `Fully-managed services` - like serverless ones—take abstraction even further, eliminating the need to provision or manage any servers at all.
- `Serveless` - You cannot see or access the underlaying infrastructure
- `Lambda` - a serverless compute service that runs code in response to events without the need to provision or manage servers
    - Maximum duration is 15 minutes
- `How Lambda works`
    - Upload code to Lambda
    - Set code to trigger from an event source
    - Run code when triggered
    - Pay only for the compute time used
- `Containers` - provide a reliable way to package your application’s code and dependencies into a single, portable unit, making them ideal for workflows that require high security, reliability, and scalability.
    - Faster and lighter than virtual machines (VMs) because they share the host computer’s operating system.
- `VMs` use a hypervisor to run full, separate operating systems, which makes them less resource-efficient and have longer startup times.
- `Amazon Elastic Container Service (ECS)` - Scalable container orchestration service for running and managing containers on AWS, like Docker containers.
    - Streamlined and integrated
    - Define some parameters
    - Fully managed service
- `Amazon Elastic Kubernetes Service (EKS)` - A fully managed service for running Kubernetes on AWS. It simplifies deploying, managing, and scaling containerized applications using open-source Kubernetes.
    - Open source platform
    - More complex
    - More control and flexibility
- `Amazon Elastic Container Registry (ECR)` - Where you can store, manage, and deploy container images. It supports container images that follow the Open Container Initiative (OCI) standards.
    - Fully managed Docker registry
    - Stores container images
- `AWS Fargate` - a serverless compute engine for containers. It works with both Amazon ECS and Amazon EKS.
    - Fargate is a container hosting platform, unlike Amazon ECS and Amazon EKS, which are both container orchestration services.
- `AWS Elastic Beanstalk` - A fully managed service that streamlines the deployment, management, and scaling of web applications.
    - Developers can upload their code, and Elastic Beanstalk automatically handles the provisioning of infrastructure, scaling, load balancing, and application health monitoring.
    - _Good for_: Deploying and managing web applications, RESTful APIs, mobile backend services, and microservices architectures, with automated scaling and simplified infrastructure management
- `AWS Batch` - A fully managed service that you can use to run batch computing workloads on AWS.
    - It automatically schedules, manages, and scales compute resources for batch jobs, optimizing resource allocation based on job requirements.
    - _Good for_: Processing large-scale, parallel workloads in areas like scientific computing, financial risk analysis, media transcoding, big data processing, machine learning training, and genomics research
- `Amazon Lightsail` - A cloud service offering virtual private servers (VPSs), storage, databases, and networking at a predictable monthly price.
    - It’s ideal for small businesses, basic workloads, and developers seeking a straightforward AWS experience without the complexity of the full AWS Management Console.
    - _Good for_: Basic web applications, low-traffic websites, development and testing environments, small business websites, blogs, and learning cloud services
- `AWS Outposts Family`- a fully managed hybrid cloud solution that extends AWS infrastructure and services to on-premises data centers.
    - It provides a consistent experience between on premises and the AWS Cloud, offering compute, storage, and networking components.
    - _Good for_: Low-latency applications, data processing in remote locations, migrating and modernizing legacy applications, and meeting regulatory compliance or data residency requirements

### Recap
This module gave you a practical understanding of AWS compute services, so you can choose the right tools for your applications. You learned when to use fully managed options like Lambda or Fargate, and when full control with Amazon EC2 made sense. You explored how containers solve deployment consistency issues and how AWS services, like Amazon ECS and Amazon EKS, simplify managing and scaling containerized applications. You also discovered services like Elastic Beanstalk, AWS Batch, Lightsail, and Outposts, and how each supported specific use cases, from basic web hosting to large-scale batch processing or hybrid cloud environments.


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


## ASSESMENT


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
