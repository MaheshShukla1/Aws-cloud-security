## [AWS CLI IAM ](https://github.com/MaheshShukla1/Aws-cloud-security/wiki/AWS-CLI-IAM)
### Cloud Computing Overview

**Definition**: Cloud computing is the on-demand delivery of IT resources such as compute power, storage, and applications over the internet with pay-as-you-go pricing.

**Traditional vs. Cloud**: Traditionally, developers had to procure, set up, and maintain physical infrastructure. Cloud computing simplifies this by providing rapid access to flexible and low-cost IT resources, allowing developers to focus on building and maintaining applications without large upfront investments.

**Key Characteristics**:

- **On-demand**: Access resources when needed.
- **Pay-as-you-go**: Pay only for what you use.
- **Scalable**: Scale resources up or down as required.
- **Global reach**: Deploy applications globally with minimal effort.

### Advantages of Cloud Computing

1. **Pay as you go**:
    
    - Only pay for the resources you use.
    - Reduces waste and optimizes costs.
2. **Economies of Scale**:
    
    - Aggregated usage leads to higher economies of scale.
    - Results in lower prices for users.
3. **Capacity Management**:
    
    - Avoid over-provisioning and under-provisioning.
    - Scale resources dynamically based on demand.
4. **Speed and Agility**:
    
    - Rapid provisioning of IT resources.
    - Reduces time to market and enhances innovation.
5. **Cost Savings**:
    
    - Focus on core business projects.
    - Reduce expenses related to maintaining physical infrastructure.
6. **Global Deployment**:
    
    - Deploy applications in multiple regions.
    - Provide lower latency and better customer experience.



### What is AWS Cloud?

**Definition**: AWS Cloud refers to Amazon’s cloud computing services, which provide on-demand delivery of IT resources over the internet with pay-as-you-go pricing. It includes a vast array of services ranging from compute power to storage, databases, analytics, networking, developer tools, IoT, security, and enterprise applications.

**Key Features**:

- **Global Infrastructure**: AWS operates from multiple data centers globally, allowing users to deploy resources in regions that best suit their needs.
- **Scalability**: Easily scale resources up or down based on demand, from serving a single customer to millions.
- **Flexibility**: Users can choose from over 200 fully-featured services to build, deploy, and manage applications efficiently.
- **Pay-as-You-Go Pricing**: Pay only for the resources consumed, with billing based on per-second or per-hour usage, depending on the service.

**Example Use Case**:

- Users can spin up virtual machines (EC2 instances) with specific configurations (e.g., CPU cores, memory) in seconds and pay for usage only when instances are running.
- Resources can be provisioned, managed, and scaled as needed, offering flexibility and cost-effectiveness.

### Benefits of AWS Cloud

1. **Cost Efficiency**:
    
    - No upfront costs; pay only for what you use.
    - Benefit from economies of scale due to AWS’s large infrastructure.
2. **Agility and Innovation**:
    
    - Rapidly deploy applications and scale globally.
    - Experiment and innovate faster with access to a wide range of services.
3. **Reliability and Security**:
    
    - Built-in security features and compliance certifications.
    - High availability and reliability with global infrastructure.
4. **Global Reach**:
    
    - Deploy applications closer to end-users for lower latency and improved performance.
    - Expand globally with minimal effort.

### Customer Use Cases

- **Startups**: Scale from initial development to large-scale operations without infrastructure constraints.
- **Enterprise**: Modernize IT infrastructure, run mission-critical applications, and reduce operational costs.
- **Public Sector**: Support government agencies with secure and compliant cloud solutions.
- **Education and Research**: Facilitate collaboration and innovation in academic and research institutions.

### Conclusion

AWS Cloud provides a robust platform for organizations of all sizes to leverage cloud computing advantages such as scalability, cost-efficiency, agility, and global reach. By utilizing AWS services, businesses can focus on innovation and growth while AWS manages the underlying infrastructure and operational aspects.


# Amazon Simple Storage Service (Amazon S3)

- **Overview**: Fully managed, serverless, low-cost object-level storage service.
- **Use Cases**: Cloud applications, dynamic websites, content distribution, mobile and gaming apps, big data analytics.
- **Key Features**:
    - **Scalability**: Store virtually unlimited amounts of data with different formats.
    - **Durability**: Highly durable with data replicated across multiple Availability Zones (AZs).
    - **Storage Classes**: Various options tailored for different access patterns and cost requirements.

#### Amazon S3 Storage Classes

1. **Amazon S3 Standard**
    
    - Suitable for dynamic websites, content distribution, mobile apps.
    - Provides high throughput and low latency.
    - Example: Storing frequently accessed media files for a social media platform.
2. **Amazon S3 Intelligent-Tiering**
    
    - Automatically moves objects between two access tiers based on changing access patterns.
    - Example: Data lakes where access patterns are unpredictable.
3. **Amazon S3 Standard-IA (Infrequent Access)**
    
    - Ideal for data that is less frequently accessed but requires rapid access when needed.
    - Example: Backup and restore systems for disaster recovery.
4. **Amazon S3 One Zone-IA**
    
    - Offers cost-effective storage in a single AWS Availability Zone.
    - Example: Storing secondary backup copies.
5. **Amazon S3 Glacier Instant Retrieval**
    
    - Low-cost archive storage with millisecond retrieval times.
    - Example: Compliance data that needs to be retained for long periods.
6. **Amazon S3 Glacier Flexible Retrieval**
    
    - Flexible retrieval options with costs balanced against access times.
    - Example: Offsite storage for disaster recovery.
7. **Amazon S3 Glacier Deep Archive**
    
    - Lowest-cost storage for long-term retention and digital preservation.
    - Example: Regulatory compliance data retention.
8. **Amazon S3 on Outposts**
    
    - Extends Amazon S3 storage to on-premises AWS Outposts environments.
    - Example: Hybrid cloud deployments requiring local data storage.

#### Benefits of Amazon S3

- **High Durability**: Data is replicated across multiple AZs.
- **Scalability**: Easily scale storage capacity up or down as needed.
- **Event Triggers**: Supports event-driven applications using AWS Lambda.
    - Example: Automatically generating thumbnails for images uploaded to S3.

#### Use Cases of Amazon S3

1. **Content Storage and Distribution**
    
    - Store and distribute large volumes of data.
    - Example: Hosting media files for a streaming service.
2. **Backup and Archiving**
    
    - Durable storage for backup data.
    - Example: Long-term storage of database backups.
3. **Build a Data Lake**
    
    - Store and analyze large datasets.
    - Example: Big data analytics platforms.
4. **Backup and Restore Critical Data**
    
    - Ensure high availability and data integrity.
    - Example: Continuous data protection for critical applications.
5. **Archive Data**
    
    - Cost-effective long-term storage for data compliance.
    - Example: Archiving financial records.
6. **Run Cloud-Native Apps**
    
    - Build scalable applications in the cloud.
    - Example: Development and deployment of serverless applications.

#### Other AWS Storage Services

### Amazon EBS (Elastic Block Store)

- **Description**: Provides persistent block-level storage volumes for use with Amazon EC2 instances.
- **Use Cases**:
    - **Database Storage**: Running databases that require consistent performance.
    - **Boot Volume**: Storing the operating system or boot applications.
    - **Transactional Workloads**: Handling transactional workloads requiring low-latency storage.
- **Features**:
    - **Snapshotting**: Allows creating point-in-time backups of volumes.
    - **Encryption**: Provides data-at-rest encryption for enhanced security.
    - **Volume Types**: Offers options like General Purpose SSD, Provisioned IOPS SSD, and Throughput Optimized HDD.

### Amazon EFS (Elastic File System)

- **Description**: Provides scalable file storage for use with Amazon EC2 instances.
- **Use Cases**:
    - **Big Data Applications**: Storing large datasets for analytics.
    - **Content Management**: Managing content repositories and media files.
    - **Web Serving**: Hosting web content that needs shared access.
- **Features**:
    - **Elasticity**: Automatically scales storage capacity up or down as files are added or removed.
    - **Compatibility**: Supports the Network File System (NFS) protocol.
    - **Performance Modes**: Offers two performance modes: General Purpose and Max I/O.

### Amazon FSx

- **Description**: Offers fully managed file systems optimized for specific workloads.
- **Supported File Systems**:
    - **Amazon FSx for Windows File Server**: Provides fully managed Windows file servers with native Windows file system compatibility.
    - **Amazon FSx for Lustre**: Offers high-performance file systems optimized for compute-intensive workloads.
- **Use Cases**:
    - **Windows File Server**: Centralized storage for Windows-based applications and workloads.
    - **Lustre File System**: High-performance computing, machine learning, and media processing.
- **Features**:
    - **Managed Service**: Handles maintenance tasks such as patching and backups.
    - **Integration**: Easily integrates with other AWS services like EC2 and S3.
    - **Cost Efficiency**: Pay only for the storage and throughput capacity you use.
