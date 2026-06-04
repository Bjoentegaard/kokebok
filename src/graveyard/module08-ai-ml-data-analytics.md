
## Module 8 - AI/ML and Data Analytics
- `Artificial Intelligence (AI)` - A broad field focused on the development of intelligent computer systems capable of performing humanlike tasks.
- `Machine learning (ML)` - is a type of AI for training machines to perform complex tasks without explicit instructions.
    - Machine learning training finds the patterns hidden in vast amounts of historical data to produce an ML model.
- `Common ML business use cases` - ML models power the Amazon.com e-commerce recommendations engine. But, ML can solve for lots of other business use cases, such as the following:
    - Predict trends - such as future stock prices.
    - Make decisions - like routing callers to the right department
    - Detect anomalies - such as bank fraud.
- `AWS AI/ML solutions` - stack is composed of the following three tiers of solutions:
    - AI services - pre-built models that are already trained to perform specific functions
    - ML services - a more customized approach with Amazon SageMaker AI where you build, train, and deploy your own ML models with fully managed infrastructure.
    - ML frameworks and infrastructure - a completely custom approach to building models using purpose-built chips that integrate with popular ML frameworks.
- `Tier 1: Pre-built AWS AI services` - The AWS AI services tier is made up of pre-built models that are already trained to perform specific functions
    - These managed services help you quickly address diverse business needs across three groups of AWS AI services.
        - Language services - are great for when you need to interpret text or speech and transform it into something meaningful.
            - `Amazon Comprehend` - uses natural language processing to extract key insights from documents.
                - Use cases: Content classification, customer sentiment analysis, and compliance monitoring
            - `Amazon Polly` - converts text into lifelike speech. It supports multiple languages, different genders, and a variety of accents.
                - Use cases: Virtual assistants, e-learning applications, and accessibility enhancements for visually impaired users
            - `Amazon Transcribe` - converts speech into text. It supports multiple languages and offers features such as speaker identification, custom vocabulary, and real-time transcription.
                - Use Cases: Customer call transcription, automated subtitling, and metadata generation for media content.
            - `Amazon Translate` - is a text translation service. This service is ideal for global communication because it supports real-time and batch text translation across multiple languages.
                - Use cases: Document translation and multi-language application integrations
        - Computer vision and search services - ideal for answering questions and gathering insights from various types of content sources such as documents, images, videos, and more.
            - `Amazon Kendra` - uses natural language processing to search for answers within large amounts of enterprise content.
                - Use cases: Intelligent search, chatbots, and application search integration
            - `Amazon Rekognition` - is a video analysis service. It can identify objects, people, text, scenes, and activities within images and videos stored in Amazon S3.
                - Use cases: Content moderation, identity verification, media analysis, and home automation experiences
            - `Amazon Textract` - detects and extracts typed and handwritten text found in documents, forms, and even tables within documents.
                - Use cases: Financial, healthcare, and government form text extraction for quick processing
        - Conversational AI and personalization services - users can interact with your apps through text and voice conversations. You can also present your customers with product recommendations personalized just for them.
            - `Amazon Lex` - you can add voice and text conversational interfaces to your applications. This service uses both natural language understanding (NLU) and automatic speech recognition (ASR) to create lifelike conversations.
                - Use cases: Virtual assistants, natural language search for FAQs, and automated application bots
            - `Amazon Personalize` - you can use historical data to build intelligent applications with personalized recommendations for your customers.
                - Use cases: Personalized streaming, product, and trending recommendations
- `Tier 2: ML services` - provides a more customized approach for customers who want a bit more control over their ML solutions without having to manage infrastructure
    - `Amazon SageMaker AI` - With this fully managed service, you can build, train, and deploy your own ML models without worrying about infrastructure
        - Key benefits:
            - Choice of ML tools - Increase innovation with different tool choices. Data scientists can use the IDE, and business analysts can use the no-code interface.
            - Fully managed infrastructure - Focus on ML model development while SageMaker AI provides you with high-performance, cost-effective infrastructure.
            - Repeatable ML workflows - Automate and standardize your MLOps practices and governance across your enterprise to support transparency and auditability.
- `Tier 3: ML frameworks and infrastructure` - Some organizations have highly specialized needs that require complete control over the ML training process. They can use in-house expertise, ML frameworks, and AWS infrastructure to develop their own ML solutions.
    - `ML frameworks` - is a software library or tool that provides experienced ML practitioners with pre-built, optimized components for building machine learning models
    - `AWS ML Infrastructure` - such as ML-optimized Amazon Elastic Compute Cloud (Amazon EC2) instances, Amazon EMR, and Amazon Elastic Container Service (Amazon ECS), can support these custom solutions.
- `Deep Learning (DL)` - is a subset of machine learning where models are trained using layers of artificial neurons that mimic the human brain.
- `Generative AI` - is a type of deep learning powered by extremely large ML models known as foundation models (FMs).
- `Foundation models (FMs)` - FMs are pre-trained on vast collections of data.
- `Large language models (LLMs)` - are a popular type of FM trained to use human language. Foundation models can also be used to create videos, images, music, and more.
- `Generative AI on AWS` - AWS offers the following types of generative AI solutions
    - `Amazon SageMaker JumpStart` - An ML hub with FMs and pre-built ML solutions deployable with a few clicks.
        - Rapid ML model deployments - Deploy pre-trained models without extensive ML expertise.
        - Custom fine-tuned solutions - Pre-trained FMs with your domain-specific data
        - ML experiments and prototypes - Compare performance for different models before committing to a specific approach.
    - `Amazon Bedrock` - A fully managed service for adapting and deploying FMs from Amazon and other leading AI companies.
        - Enterprise-grade AI - Build production-ready generative AI applications with enterprise-level security, privacy, and scalability.
        - Multimodal content generation - Create applications that can generate multiple content types, such as text and images.
        - Advanced conversational AI - Develop advanced conversational agents that connect to your enterprise data to provide accurate responses.
    - `Amazon Q` - An interactive AI assistant that can be integrated with a company's information repositories.
        - `Amazon Q Business` - can answer pressing questions, help solve problems, and take actions using the data and expertise found in your company's information repositories.
            - Use cases: Information requests, automated workflows, and insight extraction
        - `Amazon Q Developer` - provides code recommendations to accelerate development for coding languages including C#, Java, JavaScript, Python, and TypeScript applications.
            - Use cases: Faster code generation, improved reliability and security, and automated code reviews
- `Data pipelines for ETL Process` - AI/ML and traditional data analytics need clean and accessible data in a format that's usable by analytics tools and AI algorithms.
    1. _Extract_ the data from various sources and store it.
    2. _Transform_ it into a consistent, usable format for downstream tools to consume.
    3. _Load_ it into a destination system, like a data warehouse or analytics platform.
- `Data analytics` - is when analysts transform raw historical data to uncover valuable insights and trends.
    - Loan companies explaining lending decisions to customers.
    - Medical researches analyzing clinical trial data through hypothesis testing.
    - Insurance companies making their risk assessment models transparent for regulators.
    - Data ingestion services - involves moving data from source systems into your chosen storage solution.
        - `Amazon Kinesis Data Streams` - Real-time ingestion of terabytes of data from applications, streams, and sensors. This serverless service even provides automatic provisioning and scaling in on-demand mode.
        - `Amazon Data Firehouse` - An option for data ingestion in near real-time. This fully managed service provides automatic provisioning and scaling. It also delivers data within seconds to data lakes, warehouses, and analytics services.
    - Data storage services - Data can come from many different sources. To gain insights, data is commonly consolidated into a single location.
        - `Amazon S3` - This object storage service can securely house virtually any amount of structured or unstructured data. Amazon S3 is also fully elastic, automatically scaling as you add and remove data.
        - `Amazon Redshift` - is a fully managed data warehouse service that can store petabytes of structured or semistructured data. With the scalability and pay-as-you-go pricing model, organizations can cost-effectively analyze large datasets.
    - Data cataloging services - Cataloging your data with metadata provides an inventory of your organization's data.
        - `AWS Glue Data Catalog` - provides a centralized, scalable, and managed metadata repository that enhances data discovery.
    - Data processing services - Data processing services clean and transform your data so it's ready to be analyzed.
        - `AWS Glue` - is a fully managed ETL service that makes data preparation simpler, faster, and cost-effective.
        - `Amazon EMR` - is ideal for large-scale data processing and organizations with existing big data expertise. It automatically handles infrastructure provisioning, cluster management, and scaling.
    - Data analysis and visualization services - Queries and visualization tools help you to develop important insights about your data.
        - `Amazon Athena` - you can run SQL queries to analyze data in relational, nonrelational, object, and custom data sources
            - This fully managed serverless service can access data hosted on Amazon S3, on premises, or even in multi-cloud environments.
            - It offers a cost-effective solution for data analysis because you only pay for the queries you run.
        - `Amazon Redshift` - is a fully managed data warehouse solution. Its columnar storage and massively parallel processing architecture make it ideal for analyzing large datasets.
            - You can use it to perform complex SQL queries on large datasets for frequent, high-performance analytical workloads.
        - `Amazon Quicksight` - both technical and non-technical users can quickly create modern interactive dashboards and reports from various data sources without managing infrastructure
            - Amazon Q in QuickSight provides natural language queries so business analysts and users can build, discover, and share meaningful insights in seconds.
        - `Amazon OpenSearch Service` - you can search for relevant content through precise keyword matching or natural language queries.
            - Unified dashboards provide real-time data visualization as you analyze and monitor logs, traces, and metrics for various applications.

### Recap
AI/ML and data analytics are two fields that use high-quality data to analyze past events and innovate for the future. In the previous lessons, you learned how AWS AI/ML solutions help to predict future trends and automate processes. And you learned how AWS solutions can be used to analyze historical trends and develop insights from data.



# QUIZ Module 8 - AI/ML and Data Analytics

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

## ASSESSMENT

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