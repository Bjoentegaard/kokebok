
## Module 11 - Pricing and Support

- `Pay as you go` - you can adapt to changing business needs and reduce the risk of overprovisioning or missing
  capacity.
- `Save when you commit` - For certain services, such as Compute services on AWS, Savings Plans offer savings over
  On-Demand prices when you commit to a 1-year or 3-year plan.
- `Pay less by using more` - you can realize important savings as your usage increases. For some services, pricing is
  tiered, meaning the more you use, the less you pay.
- `Driving factors of cost`
    - **Compute** - you pay by a certain span of time, like by the hour or by the second. Unless you've made a
      reservation for which the cost is agreed upon beforehand, you pay from the time you launch a resource until the
      time you stop the instance.
    - **Storage** - You can choose from a broad portfolio of storage solutions with deep functionality for storing, accessing, protecting, and analyzing data. Pricing for storage largely depends on how much storage you have provisioned or how much you are using.
        - S3 six cost components when storing and managing customer data
            - Storage pricing
            - Request and data retrievel pricing
            - Data transfer and trasfer acceleration pricing
            - Data management and analytics pricing
            - Replication pricing
            - The price to process your data with Amazon S3 Object Lambda
    - **Data transfer** - In most cases, there is no charge for inbound data transfer or for data transfer between AWS services within the same Region. There are some exceptions, so be sure to verify data transfer rates before beginning.
        - _Outbound data transfer_ is aggregated across services and then charged at the outbound data transfer rate. The more data you transfer, the less you pay per gigabyte. For data storage and transfer, you typically pay per gigabyte.
- `AWS pricing and billing services` - These services are purpose-built to help you forecast, track, manage, and view your AWS costs.
    - `AWS Organizations` - apply security policies at the account level and consolidate billing with multiple accounts using a single payment method.
    - `AWS Billing and Cost Management dashboard` - centralizes cost management, showing current charges, usage, forecasts, and detailed breakdowns. It also provides tools to manage payments, view invoices, set budgets, and consolidate billing.
        - Use helpful visualizations and billing reports of monthly AWS spend.
        - Set up and manage payment methods.
    - `AWS Budgets` - helps set custom budgets and sends alerts when costs, usage, or Savings Plans and Reserved Instances (RIs) utilization or coverage exceed defined thresholds.
        - Set up alerts for when projected costs exceed predefined thresholds.
        - Forecast future expenses based on current usage trends.
    - `AWS Cost Explorer` - helps visualize, analyze, and manage AWS costs and usage with interactive graphs, reports, and forecasts. It provides insights into spending patterns, trends, and Reserved Instance recommendations.
        - Analyze historical spending trends to identify cost-saving opportunities.
        - Forecast future AWS costs based on current usage patterns to budget effectively
    - `AWS Pricing Calculator` - is a web-based planning tool that you can use to create estimates. You input specific configurations such as instance types, storage options, and data transfer volumes.
        - Estimate potential costs before deployment.
        - Compare costs of different AWS services and configurations.
- `Basic Support` - Basic plan included for all AWS customers
    - Access to documentation, whitepapers, and AWS re:Post
    - Core AWS Trusted Advisor checks
- `Developer Support` - For experimenting or testing in AWS
    - Response times: `< 24 hours` for general guidance and `< 12 hours` when system impaired
    - Core AWS Trusted Advisor checks
    - Not Technical Account Management (TAM)
- `Business Support` - Minimum recommended tier for production workloads.
    - Response times: Includes previous plan response times, `< 4 hours` when production system impaired and `< 1 hours` when production system is down.
    - Full set of AWS Trusted Advisor checks
    - No TAM
- `Enterprise On-Ramp Support` - For production and business-critical workloads needing proactive guidance.
    - Response times: Includes previous plan response times, `< 30 minutes` when business-critical system is down
    - Full set of AWS Trusted Advisor checks
    - Pool of TAMs provide proactive guidance
- `Enterprise Support` - For business and mission-critical workloads requiring highest level of support
    - Response times: Includes previous plan response times, `< 15 minutes` when business- or mission-critical system is down
    - Full set of AWS Trusted Advisor checks with prioritized recommendations by AWS account team
    - Dedicated TAM provides consultative architectural an operation guidance
- `Techinal account manager (TAM)` - included with the Enterprise On-Ramp and Enterprise Support plans. The TAM serves as your primary AWS contact, offering expert guidance on using AWS services, optimizing architectures, managing costs, and connecting you with AWS programs and experts.
- `Additional resource for your cloud journey` - AWS also provides access to other teams, resources, and documentation that you can use to support your cloud journey.
    - `AWS re:Post` - A community-driven, question-and-answer platform where users can seek help, share knowledge, and find solutions related to AWS services and technologies.
    - `AWS Trust and Safety Center` - Provides information on how to report activity or content on AWS that you suspect is abusive.
    - `AWS Solutions Architects` - Provide architectural guidance, best practice recommendations, and help in designing scalable and secure applications.
    - `AWS Professional Services` - A consulting service that offers deeper, project-based support. They help with complex migrations, security audits, performance tuning, and more.
    - `Self-Support at AWS` - Provides extensive documentation and self-support resources that you can use to research, answer a question, or troubleshoot an issue.
- `AWS Marketplace` - A digital catalog that includes thousands of software listings from independent software vendors. You can use AWS Marketplace to find, test, and buy software that runs on AWS.
    - Solutions and services offered in the AWS Marketplace include the following:
        - Software as a service (SaaS) - Business applications such as project management tools
        - Machine learning (ML) and AI - Prebuilt models for image recognition, natural language processing, and more
        - Data and analytics - Business intelligence platforms for visualization and reporting
- `AWS Partner Network (APN)` - a global community that uses AWS technologies, programs, expertise, and tools to build solutions and services for customers. Together, partners and AWS provide innovative solutions, solve technical challenges, and deliver customer value.
    - Benefits of becoming a partner
        - Funding benefits: As businesses join the AWS Partner Network and participate in specific programs available to AWS Partners, they can unlock various funding benefits to help build, market, and sell with AWS.
        - AWS Partner events: AWS Partner events include webinars, virtual workshops, and in-person learning opportunities.
        - AWS Partner Training and Certification: Take advantage of unique, partner-centered offerings from AWS Training and Certification.

### Recap
In the last few lessons, you learned about AWS pricing concepts and AWS support options. You covered fundamental pricing concepts and services. You also learned the difference between AWS Support Plans and other technical assistance resources. Finally, you applied these concepts to a real-world application by thinking about how to optimize for cost in the AWS Cloud.


# QUIZ Module 11 - Pricing and Support

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

## ASSESSMENT

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