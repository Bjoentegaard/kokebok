# Module 9 - Security
- `Authentication` - Verifying the identity of a user or entity through credentials.
    - Is the process of verifying the identity of a user or entity through credentials like a username and password combination.
    - Use case: An employee logs in to an employee portal.
- `Authorization` - Granting authenticated users with certain access rights and permissions.
    - Grants users certain access rights and permissions that determine which actions they can perform in a system or application.
    - Use case: An employee can only access their own employee records inside the employee portal.
- `Data privacy and protection` - Maintains customer trust and prevents fraud.
- `AWS security controls` - AWS offers multiple security mechanisms to help protect your cloud resources and achieve the following:
    - Prevent security incidents through proper permission and access management
    - Protect networks, application, and data
    - Detect and respond to security incidents as they occur.
- `AWS Identity and Access Managemen (IAM)` - Securely manage identities and access to AWS services and resources.
    - By default, all actions are denied.
- `Principle of least privilege` - Dictates that you should only give people and systems access to what they need and nothing else.
- `Root user` - The root user is the account owner and has permission to do anything inside the AWS account.
- `IAM user` - Represents a person or application that interacts with AWS services and resources. It consists of a name and credentials.
- `IAM Group` - Is a collection of IAM users. When you assign permissions to a group, all users in the group inherit the permissions.
- `IAM Roles` - An IAM role is a temporary identity with specific permissions. When assumed, previous permissions are dropped, and the user gains only those of the new role.
- `IAM policies` - is a JSON document that allows or denies permission to access AWS services and resources. IAM policies can also define the level of access to resources.
- `Resource` - Which AWS resource the API call is for
- Additional access management services
    - `AWS IAM Identity Center` - centralizes identity and access management across AWS accounts and applications
        - _Federated identity management is a system that allows users to access multiple applications, services, or domains using a single set of credentials._
    - `AWS Secrets Manager` - provides a secure way to manage, rotate and retrieve database credentials, API keys, and other secrets throughout their lifecycle.
        - _Secrets are confidential or private information intended to be known only to specific individuals or groups. Examples include passwords, database credentials, and API keys._
    - `AWS Systems Manager` - provides a centralized view of nodes across your organization's accounts and Regions and multi.cloud and hybrid environments.
        - _Nodes are connection points in a network, system, or structure._
- `AWS network and application protection` - automatically protects against low-level, brute-force attacks, such as DDoS, through its built-in infrastructure and network architecture.
- `AWS protection through infrastructure`
    - Security groups - only allow in proper request traffic. They operate at the AWS network level so they can shrug off massive attacks using the entire AWS Region's capacity
    - Elastic Load Balancing (ELB) - handles traffic first before handing it off, so your frontend server is not overwhelmed. Like security groups, it runs at the Region level.
    - AW Regions - The enormous capacity of Regions makes them extremely difficult to overwhelm.
- AWS protection through services
    - `AWS Shield` - designed to automatically protect AWS customers from the most common, frequently occurring types of DDoS attacks at no cost
    - `AWS WAF` - is a web application firewall that monitors network requests that come into your web applications. When a request comes into AWS WAF, it checks the IP address against a web access control list (web ACL).
- `Data Encryption` - Securing data in a way that only authorized parties can access it
    - Data encryption works like a lock and key mechanism. If you have the right key, you can access the encrypted data.
    - At rest - The data is idle and not moving, like when it's stored in a database.
    - At transit - The data is moving between locations, like when it's being sent from a database to an application. SSL/TLS certificates are used to establish encrypted network connections from one system to another.
- AWS built-in data protection
    - `Amazon S3` - all new S3 buckets have encryption configured, and all uploaded objects are encrypted at rest.
    - `Amazon EBS` - EBS volumes and snapshots can be encrypted at rest, including both boot and data volumes of an Amazon EC2 instance.
    - `Amazon DynamoDB` - Server-side encryption at rest is enabled on all DynamoDB table data using encryption keys stored in AWS Key Management Service (AWS KMS).
- `AWS Key Management Service (AWS KMS)` - use AWS KMS to create and manage cryptographic keys. These keys can then be used to encrypt and decrypt your data.
    - You can also control the use of keys across a wide range of services and in your applications.
    - _A cryptographic key is a random string of digits used for locking (encrypting) and unlocking (decrypting) data._
- `Amazon Macie` - you can monitor your sensitive data at rest to make sure it's safe. Macie uses machine learning (ML) and automation to discover sensitive data stored in Amazon S3
- `AWS Certificate Manager (ACM)` - Centralizes the management of your SSL/TLS certificates that provide data encryption in transit. It can be used to protect various AWS services and your connected on-premises resources.
    - SSL/TLS certificates are used to establish encrypted network connections from one system to another.
- Detection and response services
    - `Amazon Inspector` - Helps improve the security and compliance of applications by running automated security assessments for Amazon EC2 instances, containers, and Lambda functions.
    - `Amazon GuardDuty` - Provides intelligent threat detection across your infrastructure and resources. GuardDuty identifies threats by continuously monitoring streams of your account metadata and network activity in your environment.
    - `Amazon Detective` - After a threat has been detected, you can use Amazon Detective to further investigate the root cause. Detective helps you analyze threats with interactive visualizations contained in a unified AWS Management Console view.
    - `Amazon Security Hub` - Brings multiple security services together into a single place and format. With this service, you can quickly see your security and compliance state in one comprehensive view.

### Recap
Building and maintaining a secure environment in the cloud is an important responsibility. AWS shares this responsibility with its customers. In the previous lessons, you learned about important security concepts, mechanisms, and services that help protect your cloud resources.


# QUIZ Module 9 - Security

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

## ASSESSMENT

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