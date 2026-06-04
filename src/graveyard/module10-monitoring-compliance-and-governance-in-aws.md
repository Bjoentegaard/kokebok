# Module 10 - Monitoring, Compliance and Governance in the AWS Cloud
- `Monitoring your resources in the AWS Cloud`
    1. Secure - Protect data, systems, and infrastructure from unauthorized access, use, disclosure, disruption, modification, or destruction
    2. Monitor - Continuously observe and analyze system activity, network traffic, and security events to detect potential threats or anomalies
    3. Audit - Periodically review and assess the effectiveness of security controls and check that all requirements are met and security policies and procedures are adhered to
    4. Compliance - Help ensure that an organization's security practices and controls meet the requirements of relevant regulations, industry standards, and contractual obligations
- `Importance of monitoring` - It provides a way for you to continuously observe and analyze system activity, network traffic, and security events to detect potential threats or anomalies.
    -  Monitoring and observability are critical components for ensuring the security, availability, reliability, and performance of your cloud-based workloads and data.
- `Benefits of monitoring your cloud resources`
    - Maintain security
    - Respond proactively
    - Ensure reliability
    - Monitor costs
    - Improve performance
- `Metrics` - Variables tied to your resources
-
- `Amazon CloudWatch` - monitors your AWS resources and the applications that you run on AWS in real time.
    - you gain system-wide visibility into resource utilization, application performance, and operational health.
    - `CloudWatch metrics` - CloudWatch collects metrics from all your AWS resources, applications, and services that run on AWS and on-premises servers.
    - `CloudWatch alarms` - You can define thresholds on CloudWatch metrics and send notifications or automatically make changes to the resources.
    - `CloudWatch dashboards` - Dashboards are customizable home pages in the CloudWatch console that you can use to monitor your resources in a single view.
    - `CloudWatch logs` - Logs centralize the logs from all the systems, applications, and AWS services that you use.
    - **Benefits**: CloudWatch helps you visualize and analyze your resources, operate efficiently with automation, use an integrated view, proactively monitor, and gain insights.
- `AWS CloudTrail` - tracks user activity and API usage in the AWS Cloud, on premises, and even with other cloud providers. CloudTrail provides a detailed history of API calls, so you can track changes and identify who made them and when.
    - **Benefits**: CloudTrail provides auditing, security monitoring, and operational troubleshooting. It also helps you prove compliance and improve your security posture.
    - **Use cases:** It can be used for compliance and auditing, identifying security incidents, troubleshooting operational issues.
    - `CloudTrail events` - Event history provides a viewable, searchable, downloadable, and immutable record of the past 90 days of management events in an AWS Region. There are no CloudTrail charges for viewing event history.
    - `CloudTrail logs` - Monitors events and delivers those events as log files to your Amazon Simple Storage Service (Amazon S3) bucket. Because CloudTrail logs are securely stored, they can be used to prove compliance with regulations such as Payment Card Industry (PCI) and Healthcare Insurance Portability and Accountability Act (HIPAA).
    - `CloudTrail Insights` - Analyzes your normal patterns of API call volume and API error rates.
- `Benefits of compliance with AWS`
    - Inheriting the latest security controls that AWS uses on its own infrastructure
    - Third-party validation for thousands of global requirements
    - Streamlining and automating compliance
    - On-demand compliance reports
- `AWS Artifact` - a service that provides no-cost, on-demand access to AWS security and compliance reports and select online agreements.
    - Benefits: AWS Artifact helps you manage at scale, save time with on-demand access to compliance reports, and deploy with more confidence.
    - Use cases: It can be used to manage select online agreements and assess third-party security and compliance.
    - `AWS Artifact Agreements` - you can review, accept, and manage agreements for an individual account and for all your accounts in AWS Organizations.
    - `AWS Artifact Reports` - provide compliance reports from third-party auditors. These auditors have tested and verified that AWS is compliant with a variety of global, regional, and industry-specific security standards and regulations.
- `AWS Compliance` - contains resources to help you learn more about AWS compliance. You can read customer compliance stories to discover how companies in regulated industries have solved various compliance, governance, and audit challenges.
- `AWS Config` - a service that you can use to assess, audit, and evaluate the configurations of your AWS resources.
    - **Benefits:** AWS Config helps evaluate configurations against a desired state, manage resource configuration changes, and simplify troubleshooting and remediation.
    - **Use cases:** It can be used to continually audit security monitoring and analysis and to streamline operational troubleshooting and change management.
- `AWS Audit Manager` - A service that continually audits your AWS usage to simplify risk and compliance assessment. It helps collect evidence and manage audit data.
    - **Benefits:** Audit Manager saves time with automated evidence collection, streamlines collaboration across teams, and helps ensure integrity of audits with read-only permissions.
    - **Use case:** It can be used to automate evidence collection, continually audit to assess compliance, and deploy internal risk assessments.
- `AWS Organizations` - helps you centrally manage and govern your environment as you grow and scale your AWS resources. It helps you manage policies for groups of accounts and automate account creation.
    - Organizations provides several benefits like quickly scaling your environment by programmatically creating new AWS accounts for resources and teams.
    - It also helps by simplifying permission management through SCPs and managing and optimizing costs across your AWS accounts and resources.
- `Key concepts of Organizations`
    - `Managament account` - The management account is the central AWS account that creates and manages the organization. Responsible for overall control and governance
    - `Organizational Units (OU)`- Logical grouping of accounts in an AWS Organization. OUs can contain member accounts or nested OUs.
    - `Service Control Policies (SCP)` - a policy that lets you place restrictions on the AWS services, resources, and individual API actions that users and roles in each account can access. SCPs can be applied to either OUs or individual member accounts.
    - `Member account not in an OU` - If you have a member account that has unique requirements that do not overlap with those of an organizational unit, you can add them to the organization. They do not have to be placed under an OU.
- `AWS Control Tower` - a service you can use to enforce and manage governance rules for security, operations, and compliance at scale across all your organizations and accounts in the AWS Cloud.
    - Benefits: AWS Control Tower can help you save time while providing governance. It uses preconfigured controls, which can help you to quickly set up multi-account environments, automation with built-in governance, and integration of third-party software at scale.
    - Use cases: Use AWS Control Tower to quickly deploy applications and provision compliant AWS accounts.
- `AWS Service Catalog` - you can create, share, and organize from a curated catalog of AWS resources. You can deploy baseline networking resources and security tools for new AWS accounts so you can govern consistently.
    - Benefits: Service Catalog saves time by making it quick to find and deploy approved, self-service cloud resources. It also helps you stay agile while improving governance over resources across multiple accounts.
    - Use cases: Use it to provision resources across AWS accounts, apply access controls, and accelerate provisioning of continuous integration and continuous delivery (CI/CD) pipelines.
- `AWS License Manager` - a service that helps you manage your software licenses and fine-tune your licensing costs.
    - Benefits: License Manager helps with visibility and control, tracking and managing licenses, and reducing the risk of noncompliance with licenses.
    - Use cases: Use it to streamline license management and to simplify the Microsoft License Mobility through Software Assurance experience. You can also use it to automate the distribution and activation of software entitlements across AWS accounts for end users.
- `AWS Bring Your Own License model (BYOL)` - use existing software licenses purchased directly from vendors, such as Microsoft, on AWS services like Amazon EC2 Dedicated Hosts and Amazon WorkSpaces.
- Three governance services
    - `AWS Control Tower` - A service you can use to set up and govern a secure, compliant, multi-account AWS environment based on best practices
    - `AWS Service Catalog` - A service you can use to create, share, and organize AWS services and resources from a curated catalog that you define
    - `AWS License Manager` - A service that helps you manage your software licenses and fine-tune licensing costs
- `AWS Health` - is the go-to data source for events and changes affecting the health of your AWS Cloud resources. It notifies you about service events, planned changes, and account notifications to help you manage and take actions.
- `AWS Health Dashboard` - you can view account-specific health information and get AWS Health event updates. You can also use AWS Health programmatically using the AWS Health API, which is available with AWS Premium Support.
    - Benefits: AWS Health Dashboard provides valuable information as a data source for events and changes. It gives you timely and actionable guidance to remedy issues. It also helps manage service health and is integrated and automated to use at scale.
    - Use cases: Use AWS Health Dashboard to view account-specific health information. You can also use it to plan for lifecycle events or troubleshoot an incident.
- `AWS Trusted Advisor` - a service that provides real-time recommendations to help you optimize your AWS environment for cost, performance, security, and fault tolerance.
    - Benefits: Trusted Advisor helps you align with AWS best practices, prioritize recommendations, and optimize your AWS resources at scale.
    - Use cases: It can be used to optimize cost, efficiency, security, improve performance, and track service limits.
- `AWS IAM Access Analyzer` - provides capabilities to set, verify, and refine permissions by analyzing external access and validating that your policies match your corporate security standards.
    - Benefits: IAM Access Analyzer provides benefits like refining permissions, validating IAM policies, helping you meet your least privilege goals, and automating IAM policy reviews.
    - Use cases: It can be used to set fine-grained permissions, verify who can access what, remediate unused access, and refine and remove broad access.

## Recap
In this module, you learned the progression of securing, monitoring, auditing, compliance, and governance in the AWS Cloud. You identified services that aid in monitoring with metrics, alarms, and dashboards. You also learned about services for auditing, such as CloudTrail, and compliance, such as AWS Artifact. You reviewed several other governance and compliance services and identified the role of AWS Trusted Advisor in continuously evaluating for cost, security, performance, and more.


# QUIZ Module 10 - Monitoring, Compliance, and the Governance in the AWS Cloud

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

## ASSESSMENT

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