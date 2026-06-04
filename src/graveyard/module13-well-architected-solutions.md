## Module 13 - Well-Architected Solutions
- Development services - help developers automate CI/CD pipelines, monitor and debug applications, build GraphQL APIs, and deploy web and mobile applications on AWS.
    - `AWS CodeBuild` - fully managed continuous integration service that compiles source code, runs tests, and produces software packages for deployment. It automatically scales to meet demand, and you only pay for the build time that you use.
    - `AWS CodePipeline` - Fully managed CI/CD service that automates the build, test, and deploy phases of your release process.
    - `AWS X-ray` - A Powerful tracing, debugging and performance analysis tool that helps developers visualize application behaviour.
    - `AWS Appsync` - A fully managed GraphQL service. With Appsync, developers can create a single GraphQL API that can securely access, manipulate, and combine data from multiple data source
    - `AWS Amplify` - Helps you streamline the process of developing, deploying, and managing secure and scalable full-stack applications on AWS.
- Business application services - These services are ideal for managing business application needs such as customer service operations and email promotions.
    - `Amazon Connect` - AI-powered contact center service to efficiently set up and operate a scalable customer service call center.
    - `Amazon Simple Email Service (Amazon SES)` - A scalable and cost-effective email service provider that can be integrated into any application for reliable, high-volume email automation.
- End-user computing services - IT departments often need to provide remote access to resources like virtual desktops and applications.
    - `Amazon Appstream 2.0` - A fully managed service that streams applications from the cloud directly to any compatible device
    - `Amazon WorkSpaces` - A fully managed cloud-based desktop computing service. employees can securely access their work environment from any device with an internet connection.
    - `Amazon WorkSpaces Secure Browser (formerly Amazon WorkSpaces Web)` - A fully managed remote enterprise browser. It provides a protected environment for employees to access private websites, SaaS applications, and the public internet.
- IoT service (Internet of Things) - a network of connected physical devices embedded with sensors and software that collect and exchange data over the internet.
    - `AWS IoT Core` - A managed cloud service used to securely connect physical devices with cloud applications.
        - It helps you create efficient IoT solutions by streamlining the complex process of ingesting, processing, and acting on device data.
- `Well-Arcchitected Framwork Pillars`
    1. Operational Excellence - Focus on operations, monitoring, automation, and continuous improvement
    2. Security - Protects systems and data through best practices like least privilege and data integrity.
    3. Reliability - Emphasizes recovery planning and system adaptability to meet changing demands
    4. Performance Efficiency - Encourages using the right resources for the job and adjusting as needs evolve
    5. Cost Optimization - Helps control and reduce costs through smart provisioning and resource management
    6. Sustainability - Promotes energy-efficient design and environmentally conscious resource usage
- `AWS Well-Architected Tool (AWS WA Tool)` - A free service that helps assess and improve cloud workloads based on the six key pillars.
    - It offers workload reviews, milestone tracking, and custom lenses for tailored evaluations and improvement plans.
- `Example of enhancement`
    - Operational Excellence - EC2 Auto Scaling
    - Security - Strengthening encryption and IAM policies
    - Reliability - Amazon CloudWatch
    - Performance Efficiency - AWS Compute Optimizer
    - Cost Optimization - Savings Plans, AWS Budgets, AWS Cost Explorer
    - Sustainability - AWS Cost & Usage Report

### Recap
In this module, you explored AWS purpose-built services for development, business, and customer support. You examined the AWS Well-Architected Framework and learned about its six pillars: Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, and Sustainability. You also discovered how the AWS Well-Architected Tool helps assess and enhance workloads, so you can align with best practices. Finally, you learned about serverless architectures, highlighting how services like API Gateway, Lambda, and DynamoDB provide scalable, efficient solutions with minimal infrastructure.


# QUIZ Module 13 - Well architected Solutions

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

## ASSESSMENT

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
