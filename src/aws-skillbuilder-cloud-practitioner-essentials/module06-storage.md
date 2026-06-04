## Module 6: Storage
- `Block storage` - Provides persistent, low-latency block-level storage volumes that attach to EC2 instances like physical hard drives.
    - `Amazon EC2 instance store`- An unmanaged non-persistent, high-performance block storage directly attached to EC2 instances for temporary data.
        - Is best for temporary memory-based storage needs like buffers, caches, and scratch data. It is not recommended for applications that require data retention.
        - Automatically available storage - Instance store volumes are temporary, high‑performance block storage physically attached to the host, included at no extra cost on many EC2 instance types and erased when the instance stops.
        - Cost effective - Is included in the instance price, making it ideal for temporary data like caches or buffers and helping reduce costs for workloads that don’t need persistent storage.´
        - EC2 instance store provides ultra‑low latency and high I/O performance by being directly attached to the host server, making it ideal for temporary fast‑processing data.
    - `Amazon Elastic Block Store (EBS)` - A managed service that provides persistent block storage volumes for EC2 instances, offering various types for different workloads
        - EBS volumes act like external hard drives, offering consistent and low-latency performance for workloads like databases and file systems.
        - Use cases - Some practical use cases of Amazon EBS include database hosting, backup storage for applications, and rapid deployment of development environments using volume snapshots.
        - Data migration - EBS volumes can be easily migrated between Availability Zones using snapshots. The snapshots provide a simple way to move data across regions or create copies.
        - Instance type changes - EBS volumes are separate from EC2 instances, so you can easily attach them to other instance types and change sizes without losing data.
        - Disaster recovery - EBS snapshots offer reliable, automated backups that can be restored across regions for fast recovery during emergencies.
        - Cost optimization - EBS volumes can be resized or changed to different types without downtime, letting you match storage to usage needs.
        - Performance tuning - Amazon EBS provides multiple volume types and adjustable performance to suit varying workload and IOPS requirements.
- `Object storage` - is a data storage architecture that manages data as objects in a flat address space.
    - It offers unlimited scalability so you can store vast amounts of unstructured data without worrying about capacity constraints.
    - Object storage provides enhanced metadata capabilities to provide more efficient data management, search, and analytics across massive datasets.
    - **`Amazon Simple Storage Service (S3)` - A fully managed scalable object storage service for storing and retrieving any amount of data from anywhere.**
        - Store data as objects -> Store object in buckets
        - Upload a maximum size of 5 TB
        - Create multiple buckets
        - Offers features like versioning, lifecycle management, and various storage classes to optimize costs.
        - Each object typically includes the data itself, metadata, and a unique identifier, or key.
        - Each Amazon S3 object is uniquely identified within a bucket by its key, which is essentially its file name.
        - Objects also have properties like version ID, access control information, and user-defined metadata.
- `File storage` - file storage services provide shared file systems accessible over networks, so multiple users and applications can access the same data simultaneously.
    - They offer scalability and flexibility so you can expand storage capacity as needs grow without managing physical infrastructure.
    - `Amazon Elastic File System (EFS)` - A fully managed, scalable NFS file system for use with AWS Cloud services and on-premises resources.
        - Multiple instances reading and writing simultaneously
        - EFS is designed to support a wide variety of workloads and can be accessed by multiple EC2 instances simultaneously.
        - Benefits:
            - Multi-AZ redundancy - automatically replicates data across multiple Availability Zones in a region for high availability.
            - Shared access - supports thousands of concurrent NFS connections, so multiple EC2 instances can access the same file system simultaneously.
            - Elastic storage - automatically grows and shrinks as you add and remove files, with no need to provision or manage storage capacity.
    - `Amazon FSx` - A fully managed file storage services for popular file systems like Windows, Lustre, and NetApp ONTAP.
        - Benefits:
            - File system integration - Supports industry-standard file system protocols, allowing convenient integration with your existing applications, workflows, and development tools.
            - Managed infrastructure - Reduces the complexity of managing infrastructure while delivering the features and capabilities of traditional file systems.
            - Scalable storage - Adjusts resources dynamically, eliminating the need for complex capacity planning and manual infrastructure management.
            - Cost effective - has a pricing model and automated tiering options that optimize costs by charging only for used storage and moving infrequently accessed data to lower-cost tiers.
- `NFS` - Network File System
- `AWS Storage Gateway` - A fully managed, hybrid-cloud storage service that provides on-premises access to virtually unlimited cloud storage.
- `AWS Elastic Disaster Recovery` - A fully managed service that streamlines the recovery of your physical, virtual, and cloud-based servers into AWS.
- `Amazon EBS Snapshots` - Point-in-time backups of EBS volume. They can be used for disaster recovery, data migration, volume resizing, and for creating consistent backups of production workloads.
    - EBS snapshots are incremental, so they only save the blocks on the volume that have changed after your most recent snapshot.
    - Can be used to create multiple new volumes, and new volumes created from a snapshot are an exact copy of the original volume at the time the snapshot was taken.
    - Snapshots of EBS volumes are stored redundantly in multiple Availability Zones using Amazon S3.
    - Benefits
        - Data protection and recovery - Enable fast data recovery from corruption, accidental deletion, or system failures using point-in-time backups.
        - Operational flexibility - Enable operations like cross-Region data migration, volume resizing, volume cloning, and sharing data across AWS accounts.
        - Cost effective - Use incremental backup technology, storing only changed blocks after the initial backup, reducing storage costs and backup time.
- `Amazon Data Lifecycle Manager` - You can automate the creation, retention, and deletion of EBS snapshots using Amazon Data Lifecycle Manager.
    - Schedule automatic snapshot creation
    - Set retention policies
    - Manage snapshot lifecycle
    - Apply consistent backup policies
- `AWS S3 Benefits`
    - Virtually unlimited storage - no fixed storage limit, scaling automatically to accommodate any amount of data you need to store.
    - Object lifecycle management - lifecycle policies automatically move objects between storage classes based on your defined rules, optimizing costs over time.
    - Broad range of use cases - supports a wide range of use cases for both cloud-based applications and traditional on-premises workloads. Amazon S3 is commonly used for content distribution, hosting static websites, and delivering media files.
- `S3 Security and privacy management`
    - Everything you store in Amazon S3 is private by default
    - **Bucket policies** - Resource-based policies that can only be attached to S3 buckets. An S3 bucket policy specifies which actions are allowed or denied on the bucket, in addition to every object in that bucket.
    - **Identity-based policies** - Permissions that control what actions users, groups, or roles can perform on S3 resources are attach directly to identities rather than to the S3 resources themselves
    - **Encryption** - Provides encryption capabilities to protect data both at rest and in transit.
- `Amazon S3 storage classes and uses cases`
    1. `S3 Standard` - General-purpose storage for cloud applications, dynamic websites, content distribution, mobile and gaming applications, and big data analytics
    2. `S3 Intelligent-Tiering` - This tier is useful if your data has unknown or changing access patterns. Stores objects in three tiers: a frequent, an infrequent, and an archive instant access tier.
    3. `S3 Standard Infrequent Access (Standard-IA)` - For infrequently accessed data that still needs fast retrieval. Provides the same durability, throughput, and low latency as S3 Standard, but at a lower storage cost with a retrieval fee—ideal for long-term backups and disaster recovery.
    4. `S3 One Zone Infrequent Acces (One Zone-IA)` - Stores data in a single Availability Zone, reducing costs compared to S3 Standard-IA, which uses three zones.
    5. `S3 Express One Zone` - It was purpose-built to deliver consistent single-digit millisecond data access for your most frequently accessed data and latency-sensitive applications. Delivers data access speed up to 10x faster and request costs up to 80% lower than S3 Standard.
    6. `S3 Glacier Instant Retrieval` - Archiving data that is rarely accessed and requires millisecond retrieval.
    7. `S3 Glacier Flexible Retrieval` - Offers low-cost storage for archived data that is accessed 1–2 times per year. With S3 Glacier Flexible Retrieval, your data can be accessed in as little as 1–5 minutes using an expedited retrieval.
    8. `S3 Glacier Deep Archive` - is S3’s lowest-cost storage class, built for long-term retention (7–10+ years) and regulatory compliance. Ideal for rarely accessed data—retrieval takes about 12 hours—such as archives in finance, healthcare, or public sectors.
    9. `S3 Outpost` - Delivers object storage to your on-premises AWS Outposts environment using Amazon S3 APIs and features, and serves workloads with local data residency requirements.
- `S3 Lifecycle` - Automating object storage tier config
    - _Transition actions_: define when objects should transition to another storage class.
    - _Expiration actions_: define when objects expire and should be permanently deleted.
    - Use cases
        - _Periodic logs_: If you upload periodic logs to a bucket, your application might need them for a week or a month. After that, you might want to delete them.
        - _Data that changes in access frequency_: Some documents are frequently accessed for a limited period of time. After that, they are infrequently accessed. At some point, you might not need real-time access to them.
- `Amazon EFS storage classes`
    - Standard Storage Classes - Offer Multi-AZ resilience and the highest levels of durability and availability.
    - One Zone Storage Classes - Provide additional savings by saving your data in a single Availability Zone.
    - Archive Storage Class - Is cost-optimized for data that is accessed only a few times a year or less and that does not need the sub-millisecond latencies of EFS Standard.
- `EFS Lifecycle` - You can create lifecycle policies that determine when and how files transition between different storage tiers.
    - Transition to IA - This policy instructs lifecycle management when to move files into the Infrequent Access storage, which is cost-optimized for data that is accessed only a few times each quarter.
    - Transition to Archive - This policy instructs lifecycle management when to move files into the Archive storage class, which is cost-optimized for data that is accessed only a few times each year or less.
    - Transition to Standard - This policy instructs lifecycle management whether to transition files out of IA or Archive and back into Standard storage when the files are accessed in the IA or Archive storage.
- `Amazon FSx file systems`
    - Windows File Server
    - NetApp ONTAP
    - OpenZFS
    - Lustre
- `AWS Storage Gateway` - Is a hybrid cloud storage service that makes it possible to seamlessly integrate on-premises environments with AWS Cloud storage.
    - Benefits
        - Seamless integration
        - Improved data management
        - Local caching
        - Cost optimization
- `Gateway types` - offers three distinct types of gateways to meet different hybrid storage needs
    - Amazon S3 File Gateway - Bridges your local environment with Amazon S3. It provides on-premises applications with access to virtually unlimited cloud storage through familiar file protocols.
    - Volume Gateway - Lets you create virtual storage volumes with local access, bridging on-premises infrastructure and AWS Cloud by presenting cloud data as iSCSI volumes.
    - Tape Gateway - Makes it possible to replace physical tape infrastructure with virtual tape capabilities while benefitting from the durability and scalability of AWS Cloud storage.
- `Elastic Disaster Recovery` - replicates critical workloads to AWS with minimal downtime. Your servers' block-level data is continuously replicated to AWS, making it ideal for uses that require robust disaster recovery solutions.
    - Supports both physical and virtual servers
    - Benefits:
        - Business resilience - Maintain business operations with continuous block-level data replication and the ability to recover workloads within minutes during disruptions.
        - Streamlined disaster recovery - Automate disaster recovery processes through an intuitive console, reducing complex manual configurations and minimizing the risk of human error.
        - Cost optimization - Eliminate expensive secondary data centers and pay only for what you use, with minimal upfront investment and no standby infrastructure costs.
    - Use cases
        - Healthcare data protection
        - Financial services continuity
        - Manufacturing operations recovery

### Recap
In this module, you learned about the diverse storage options available in AWS, starting with block storage services like Amazon EC2 Instance Store and Amazon EBS. You learned how Amazon EBS provides persistent block storage volumes for EC2 instances, while EC2 instance store offers temporary block-level storage. You learned how to use EBS snapshots and AWS Data Lifecycle Manager for automated backup management and data protection.

You then examined Amazon S3, a highly scalable object storage service that serves as a foundation for many cloud storage needs. You delved into file storage solutions, including Amazon Elastic File System (Amazon EFS) for Linux-based workloads and Amazon FSx for Windows, Lustre, OpenZFS, and NetAPP ONTAP file systems. Finally, you learned about AWS Storage Gateway, which bridges on-premises environments with AWS storage services to enable hybrid cloud storage architectures.



# QUIZ Module 6 - Storage

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

## ASSESSMENT

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