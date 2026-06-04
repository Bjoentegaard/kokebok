# Module 7: Databases
- `Relational Databases` - store data in a way that relates it to other pieces of data, and they use structured query language, or SQL, to manage and query data.
- `Amazon Relational Database Service (Amazons RDS)` - Managed relational database service that handles routine database tasks such as backups, patching, and hardware provisioning.
    - Supports multiple database instance class types that optimize for memory, performance, or input/output (I/O).
    - Supports different database engines, including Amazon Aurora, MySQL, PostgreSQL, Microsoft SQL Server, MariaDB, and Oracle Database.
    - Benefits:
        - Cost optimization - Eliminates the high upfront costs of purchasing and maintaining database hardware infrastructure. You only pay for the compute and storage resources that you consume through a flexible pay-as-you-go model.
        - Multi-AZ deployment - Improves database reliability through Multi-AZ deployments. It automatically replicates data to a standby instance in a different Availability Zone.
        - Perfomance optimization - enhances database performance through automated management of resource allocation, monitoring, and optimization tasks.
        - Security controls - enhances database security through multiple layers of protection, including VPC isolation as well as encryption at rest and in transit.
- `AWS Database Migration Service (AWS DMS)` - Helps you migrate databases quickly and securely to AWS with minimal downtime by continuously replicating data during the migration process.
- `Amazon Aurora` - Managed relational database designed to help reduce unnecessary I/O operations. It's compatible with MySQL and PostgreSQL, provides high performance and availability, and automatically scales alongside your workloads.
    - High performance and availability - Delivers up to five times the throughput of standard MySQL and three times the throughput of PostgreSQL. It uses a distributed storage system across multiple nodes to provide high performance and availability.
    - Automated storage and backup management - Automatically grows storage from 10 GB to 128 TB based on your actual data usage, which eliminates guesswork in capacity planning.
    - Advanced replication and fault tolerance - Replicates data across three Availability Zones with six copies of data, and provides 99.99% availability. It automatically detects database failures and redirects traffic to healthy replicas without data loss.
- `Querying Relation Data` - Involves retrieving, manipulating, and managing information stored in relational databases.
    - MySQL
    - PostgreSQL
    - Microsoft SQL Server
- `Structured Query Language (SQL)` - Is a programming language for storing and processing information in a relational database
- `NoSQL databases` - are sometimes referred to as non-relational databases. Instead of row and column relationships, NoSQL databases build a structure for the data that they contain using key-value pairs instead
    - With key-value pairs, data is organized into items identified by unique keys.
- `Amazon DynamoDB` - is a fully managed NoSQL database service that provides fast and predictable performance for both document and key-value data structures.
    - Data = items = set of attributes
    - Attribute = name + value
    - Add/remove attribute any time
    - Benefits:
        - Scalability with provisioned capacity - Automatically scales throughput up or down based on actual usage, which ensures consistent performance without manual intervention.
        - Consistent high perfomance - Delivers single-digit millisecond response times at any scale, which makes it ideal for high-performance applications.
        - High availability and durability - Delivers 99.999% data availability by replicating data across three distinct facilities within each AWS Region.
        - Data encryption - Offers comprehensive encryption capabilities to protect information both at rest and in transit. All data is automatically encrypted behind the scenes before being written to the storage layer.
- `In-memory caches` - Is a high-speed storage layer that temporarily stores frequently accessed data in a computer's main memory, or RAM.
- `Amazon ElastiCache` - Is a fully managed in-memory caching service that was built to help reduce the complexity of administering in-memory caching systems.
    - It automatically detects and replaces failed nodes, which makes it ideal for applications that need consistent high performance.
    - Benefits:
        - High performance for Redis, Valey, or Memchached instances - simplifies deploying and managing in-memory caches with automated provisioning, patching, monitoring, and seamless scalability.
        - High availability - Provides high availability by constantly monitoring primary nodes for potential failures.
        - Replication across multiple AZ - Enables automatic replication across multiple Availability Zones to protect against infrastructure failures.
        - Data encryption - Supports data encryption mechanisms to safeguard sensitive information throughout its lifecycle.
- `There is no one-size-fits-all database for all purposes`
- `Amazon DocumentDB` - is fully managed service designed to handle semistructured data, which is information that doesn't conform to rigid relational schemas.
    - is a MongoDB-compatible database, so it manages JSON-like documents with dynamic schemas.
    - is perfect for applications requiring frequent schema changes and document-oriented data. Unlike relational databases or nonrelational databases, you can quickly iterate without relying on predefined schemas.
    - Use cases:
        - Content management systems
        - Catalog
        - Inventory management, and user profile and personalization systems.
    - Benefits:
        - MongoDB compability - Is fully compatible with MongoDB workloads and supports MongoDB APIs, drivers, and tools.
        - Performance and scalability - Automatically scales storage up to 64 TB in 10 GB increments based on your application needs.
        - Increased read throughput - Improves read throughput for high-volume applications by creating up to 15 replica instances that share underlying storage.
- `AWS Backup` - Streamlines data protection across various AWS resources and on-premises deployments by providing a single dashboard for monitoring and managing backups.
    - It eliminates the complexity of managing multiple backup strategies by supporting multiple storage types, including Amazon EBS volumes, Amazon EFS file systems, and various databases.
    - Benefits:
        - Centralized backup management - Provides a single dashboard to manage backups across multiple AWS services and accounts.
        - Cross-region backup redundancy - Enables automatic replication of backup data across different AWS Regions for disaster recovery purposes.
        - Streamlined regulatory compliance - Maintains detailed audit logs and reports to demonstrate compliance with regulatory requirements.
- `Amazon Neptune` - is a fully managed, purpose-built graph database service that manages highly connected data sets, like those used in social networking applications.
    - It excels at understanding complex relationships that are difficult to identify in traditional relational databases like user connections, friend networks, and interaction patterns.
    - Benefits:
        - Purpose-built for complex relationships - It supports both property graph and resource description framework, or RDF, models making it ideal for relationship mapping and pattern matching applications.
        - High performance and scalability - Delivers consistent performance at scale, processing billions of relationships in milliseconds. It automatically grows storage up to 64 TB based on your application needs.

### Recap
In this module, we explored the managed relational database capabilities of Amazon RDS and Amazon Aurora. You learned how AWS DMS facilitates seamless database migrations, and DynamoDB provides insights into NoSQL database solutions for scalable applications.

We covered the in-memory caching capabilities of ElastiCache and the MongoDB-compatible document database features of Amazon DocumentDB. We examined the comprehensive data protection strategy across AWS services offered by AWS Backup. And finally, we concluded with the powerful graph database capabilities of Neptune for complex relationship queries.


# QUIZ Module 7 - Databases

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

## ASSESSMENT

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
