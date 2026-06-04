# Module 12 - Migrating to the AWS Cloud
- `Three phases of the migration process`
    - Assess - you build the business case for the migration and assess your readiness.
        - Pre-migration Assessment tools: `Migration Evaluator`
    - Mobilize - you prepare the organization and mobilize the resources needed for the migration.
        - Migrations tools: `AWS Application Discorvery Service` and `AWS Migration hub`
    - Migrate and modernize - you use your strategy, plan, and the best practices to migrate and modernize.
        - Migration tools: `AWS Application Migration Service` and `AWS Database Migration Service`
        - Data transfer tools: `AWS DataSync`, `AWS Transfer Family` and `AWS Snow Family`
- `AWS Cloud Adoption Framework (AWS CAF)` - a framework that brings AWS experience and best practices to companies preparing to migrate to the AWS Cloud.
    - Benefits: AWS CAF provides benefits for migrations to reduce business risk and improve sustainability and corporate transparency.
    - Use cases: You can use AWS CAF to migrate technology like legacy infrastructure and applications.
- `Six perspectives of AWS CAF`
    - Business - makes sure that IT aligns with business needs and that IT investments link to key business results.
        - Common Business perspective roles:
            - Business managers
            - Finance managers
            - Budget owners
            - Strategy stakeholders
    - People - supports development of an organization-wide change management strategy for successful cloud adoption.
        - helps human resources (HR) employees prepare their teams for cloud adoption by updating organizational processes and staff skills to include cloud-based competencies.
        - helps to move from a model that separates business and IT strategies into a business model that integrates IT strategy.
        - Common People perspective roles:
            - Human resources
            - Staffing
            - People managers
    - Governance - focuses on skills and processes to align IT strategy with business strategy.
        - Common Governance perspective roles:
            - Chief information officer (CIO)
            - Program managers
            - Enterprise architects
            - Business analysts
            - Portfolio managers
    - Platform - includes principles and patterns for implementing new solutions in the cloud and migrating on-premises workloads to the cloud.
        - Use a variety of architectural models to understand and communicate the structure of IT systems and their relationships.
        - includes principles for implementing new solutions and migrating on-premises workloads to the cloud.
        - Common Platform perspective roles:
            - Chief technologu officer (CTO)
            - IT managers
            - Solutions architects
    - Security - makes sure that the organization meets security objectives for visibility, auditability, control, and agility.
        - Common Security perspective roles:
            - Chief information security officer (CISO)
            - IT security managers
            - IT security analysts
    - Operations - helps you to enable, run, use, operate, and recover IT workloads to the level agreed upon with your business stakeholders.
        - focuses on operating and recovering IT workloads to meet the requirements of the business stakeholders.
        - Define how day-to-day, quarter-to-quarter, and year-to-year business is conducted. Align with and support the operations of the business.
        - Common Operations perspective roles:
            - IT operations managers
            - IT support managers
- Seven Migration Strategies
    - `Relocate` - Changing the hosting location to the cloud. Moving VM or container to the cloud
    - `Rehost` - Lift-and-shift, moving application without changes.
    - `Replatform` - Lift, tinker and shift, involves makin a few cloud optimizations to relize a tangible benefit.
    - `Refactor` - Rearchitecting, involves reimagining how an application i architected and developed by using features built for the cloud.
        - Refactoring is driven by a strong business need to add features, scale, or improve performance that would otherwise be difficult to achieve in the application’s existing environment.
    - `Repurchase` - Moving from a traditional license to a software-as-a-service (SaaS) model.
    - `Retain` - Consists of keeping application that are critical for the business in the source environment.
    - `Retire` - The process of removing applications that are no longer needed.
- `Migration Evaluator` - a migration assessment service that helps you create a business case for AWS Cloud planning and migration. It does this with a data driven approach, analyzing your current state, target state, and developing a migration readiness plan with projected cloud costs.
    - Benefits: The benefits include removing the guesswork when migrating. It provides visibility into multiple cost-effective cloud migration scenarios.
    - Use cases: You can use Migration Evaluator to conduct broad-based discovery, take a snapshot of your current on-premises footprint to fine-tune licensing, view server dependencies, and gain visibility into multiple migration scenarios.
- `Application Discovery Service` - discovers on-premises server inventory and connections. It gathers configuration, performance, and connection details for both servers and databases to create a detailed migration plan.
    - Benefits: With Application Discovery Service, you get a comprehensive snapshot of your on-premises inventory.
    - Use cases: You can use the AWS Application Discovery Service to conduct discovery and inventory, map the connections and dependencies, and generate a migration plan.
- `Migration Hub` - a centralized hub to take you from discovery, assessment, planning, and execution of your migration. It provides tools, guidance, and automated recommendations to collaborate with your team and track your migration.
    - Benefits: With the Migration Hub, you have one location to go for your migration and, expert guidance in the form of prescriptive journey templates.
    - Use cases: You can use Migration Hub for migration assessment and planning and migration completion and collaboration with teams.
- `Application Migration Service` - a tool to move and improve your on-premises and cloud-based applications. It helps customers streamline, expedite, and reduce the cost of migrating and modernizing applications.
    - Benefits: The benefits include support to migrate from any source infrastructure that runs a supported operating system (OS).
    - Use cases: You can use the Application Migration Service for on-premises applications running on physical servers or infrastructure, cloud-based applications, or moving between AWS Regions.
- `AWS Migration and Modernization Competency Partners` - Partners who specialize in specific phases of the migration or the type of help you need.
- `AWS Database Migration Service (AWS DMS)` - Makes it possible to quickly and securely migrate databases and perform ongoing data replication tasks for live databases and data warehouses.
    - Benefits: AWS DMS provides benefits for migrating databases including maintaining high availability and low downtime during the migration process. It supports homogenous and heterogenous migrations. It also makes it possible to migrate terabyte sized databases at a low cost.
    - Use cases: You can use AWS DMS to move to managed databases, remove licensing costs, replicate ongoing changes in your database, and improve integration with data lakes.
- `AWS Schema Conversersion Tool (AWS SCT)` - makes it possible to convert database schemas and code objects (like stored procedures, views, and functions) from one database engine to another.
    - Benefits: AWS SCT provides benefits to simplify database migrations by automating schema analysis, recommendations, and conversion at scale. It is compatible with popular databases and analytics services as source and target engines.
    - Use cases: You can use AWS SCT to move from commercial databases to open source databases. You can also use it for migrating large data warehouse workloads and modernizing or updating database schemas in place.
- Transferring data online to and from the AWS Cloud
    - `AWS Datasync` - is specifically designed for automating and accelerating data transfer.
        - DataSync simplifies and accelerates moving large amounts of data between on-premises storage and AWS storage services like Amazon Simple Storage Service (Amazon S3).
        - It automates many aspects of the transfer process, including running instances, encryption, and network optimization.
        - Benefits: The benefits include streamlining and accelerating secure data migrations. DataSync manages data movement workloads with bandwidth throttling, migration scheduling, task filtering, and task reporting.
        - Use cases: You can use DataSync to migrate your data, archive your cold data, and manage hybrid data workflows.
    - `AWS Transfer Family` - makes it possible to seamlessly manage and share data with simple, secure, and scalable file transfers.
        - makes it possible to seamlessly manage and share data with simple, secure, and scalable file transfers.
        - Benefits: The benefits include simplifying the process of setting up and managing file transfers and reducing the need for complex infrastructure management.
        - Use cases: You can use the Transfer Family to modernize and manage your file transfers, simplify data sharing with your workforce and partners, and integrate transactional business data into a unified data lake.
    - `AWS Direct connect` - a service that makes it possible for you to establish a dedicated private connection between your network and virtual private cloud (VPC) in the AWS Cloud.
        - Because it is your dedicated connection, it is a fast, reliable, and secure way to transfer your data or files.
        - Benefits: Direct Connect helps reduce network costs and increase amount of bandwidth.
- Transferring data offline
    - `Snowball Edge Storage Optimized devices` - a great solution for offline data migration where connecting to the internet might not be an option.
        - Benefits: The benefits include delivering better compute performance and larger storage capacity with gigabytes of data per second for data migration workloads with offline requirements.
        - Use cases: You can use Snowball Edge devices for data migration when offline migration is required. They can also be used for edge computing when a secure, rugged device is needed.

### Recap
In this migration module, you identified the AWS Cloud Adoption Framework (AWS CAF), the seven migration strategies, and migration services to migrate applications, databases, and data.


# QUIZ Module 12 - Migrating to the AWS Cloud


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

## ASSESSMENT

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