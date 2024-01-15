## AWS Quiz with Explanations

### 1)
Your organization is expanding its AWS footprint into new regions, but they want the VPCs to communicate with each other. 

**Which service or feature can enable communication between two VPCs in different regions?**
- [ ] Private Subnet
- [x] VPC Peering
- [ ] Security Group
- [ ] Internet Gateway

**Explanation:**
VPC Peering allows communication between two VPCs in different regions, enabling secure and direct connectivity.

### 2)
A customer wants to purchase Savings Plans but anticipates their initial selection of AWS Region may change.

**Which Savings Plans option(s) should she select?**
- [ ] EC2 Instances Savings Plans and Amazon SageMaker Savings Plans
- [ ] Compute Savings Plans and Amazon SageMaker Savings Plans
- [ ] Only EC2 Instances Savings Plans.
- [x] Compute Savings Plans and EC2 Instances Savings Plans

**Explanation:**
Compute Savings Plans and EC2 Instances Savings Plans are flexible and region-independent, making them suitable for changing AWS Regions.

### 3)
Your organization wants to be able to re-use Lambda functions and ensure the same result every time.

**What coding principle would you use to write your functions to ensure that your code properly validates events and handles duplicate events in the same way?**
- [ ] Expressions
- [ ] Layers
- [x] Idempotence
- [ ] Quotas

**Explanation:**
Idempotence ensures that the same operation produces the same result, making Lambda functions reusable and consistent.

### 4)
A web application is hosted on a single c6i.large instance. The instance has been flagged as oversized due to consistently low CPU utilization. The OS and application are stored on an EBS volume. The AMI is using an Amazon Linux 2 x86_64 kernel. The instance has a single Elastic Network Interface (ENI) in a public subnet, and has an associated Elastic IP address (EIP). A solutions architect reviewed the instance and application metrics and determined that a c7g.medium instance is the optimal instance type and size for this workload. The instance needs to keep its public IPv4 address through the change.

**Which component is MOST likely to need re-architecting to be able to change to the new instance type?**
- [ ] Elastic Network Interface (ENI)
- [ ] Amazon EBS
- [ ] Elastic IP Address (EIP)
- [x] Amazon Machine Image (AMI)

**Explanation:**
To change the instance type, the new AMI needs to be created based on the optimized c7g.medium instance type.

### 5)
You have been asked to run a compute-intensive workload that requires a minimum of 8vCPUs and 32GiB of memory.

**Which instance type best fits this description?**
- [ ] M7i.2xlarge
- [ ] C6a.xlarge
- [ ] R6i.4xlarge
- [x] R6a.4xlarge

**Explanation:**
The R6a.4xlarge instance type provides 8vCPUs and 32GiB of memory, meeting the specified requirements.

### 6)
The finance department seeks your help determining the cost impact per application before and after any rightsizing activities. Each application has many Amazon EC2 instances.

**What is your BEST recommendation to meet the requirements?**
- [ ] Recommend that all finance department instances are tagged with a tag called Finance with a unique tag value per application.
- [x] Recommend that all finance department instances be tagged with a user-defined cost allocation tag called Finance with a unique tag value for each application.
- [ ] Recommend that the finance department use a system-defined cost allocation tag.
- [ ] Use a unique instance naming scheme for each application.

**Explanation:**
Using user-defined cost allocation tags provides granularity to assess cost impact per application during rightsizing activities.

### 7)
Your organization has been running several Amazon EC2 instances. You are looking for new instance types that are more cost-effective and improve performance.

**What is the term given to new instance types that have been developed to be better performing and cost-effective compared to earlier AWS instance releases?**
- [ ] AWS S3 Intelligent-Tiering
- [ ] AWS Cost Explorer Recommendations
- [ ] Compute Savings Plans
- [x] Price-To-Performance Ratio

**Explanation:**
Price-To-Performance Ratio refers to new instance types designed for improved performance and cost-effectiveness.

### 8)
You have been asked to modify an Amazon EC2 instance for an Instance backed by an Amazon EBS Volume.

**In planning for the change, what is the first thing you must do before changing the instance type?**
- [ ] Backup the EBS Volume associated with the instance.
- [ ] Identify the service level agreements (SLAs) with your internal user groups to initiate planned downtime.
- [x] Determine if the new instance type selected supports EBS optimization.
- [ ] Stop the instance.

**Explanation:**
Ensuring EBS optimization compatibility is crucial before changing the instance type.

### 9)
A software engineer has deployed 100 Amazon EC2 instances split across 2 Availability Zones to host multiple internal applications. Currently, a snapshot is taken manually each day, creating long delays.

**Which tool can automate the backup of Amazon Machine Images (AMIs) and Amazon Elastic Block Store (EBS) with minimum operational overhead?**
- [ ] Create a Lambda function that takes a snapshot and stores it Amazon S3
- [ ] Integrate Amazon S3 with Amazon EC2 and enable automatic snapshots
- [x] Use Amazon Data Lifecycle Manager
- [ ] Create a Step Function to automate the snapshot lifecycle

**Explanation:**
Amazon Data Lifecycle Manager can automate AMI and EBS backup tasks with minimal operational overhead.

### 10)
A company wants to deploy a high-speed memory application for delivering fast-performance workloads processing large data sets in memory.

**What instance family will be BEST suited for this use case?**
- [x] R5
- [ ] T2
- [ ] C4
- [ ] M3

**Explanation:**
The R5 instance family is optimized for high-speed memory applications and fast-performance workloads.

### 11)
Your company wishes to utilize an open-source file system with your Amazon EC2 instance.

**Which file storage solution should they utilize?**
- [ ] Amazon RDS
- [ ] Amazon EFS
- [ ] Amazon S3
- [x] Amazon FSx

**Explanation:**
Amazon FSx is designed for open-source file systems and is suitable for use with Amazon EC2 instances.

### 12)
Anycompany uses several Amazon EC2 instances to manage and push the regular updates to a fleet of remote field sensors. Each remote device sensor has unique credentials to communicate with the Amazon EC2 instances. The security engineer has been instructed to ensure that access to specific credentials is independently auditable and secretly stored.

**What is the MOST cost-effective way to manage the storage of credentials?**
- [ ] Store the credentials in the AWS Systems Manager Parameter Store.
- [ ] Deploy SSM agent to store the credential on Amazon EC2.
- [ ] Deploy the AWS CloudHSM device to store and audit secrets.
- [x] Use AWS Secret Manager.

**Explanation:**
AWS Secret Manager is a cost-effective solution for managing and securely storing sensitive credentials with auditability.

### 13)
You've created a Lambda function successfully invoked for the first few attempts. After some time, you begin to see connection errors.

**What would you add to your Lambda function runtime to maintain your persistent connection?**
- [ ] Environment Variables
- [ ] Java Runtime Libraries
- [ ] Keep-Alive Directive
- [ ] Lambda Handler

**Explanation:**
To maintain a persistent connection, the Keep-Alive Directive should be added to the Lambda function runtime.

### 14)
Your organization is setting up a website to launch a new marketing campaign. The team needs help in budgeting costs.

**What are the primary cost drivers for the campaign? (Select THREE)**
- [ ] Storage
- [ ] Compute
- [ ] Outbound Data Transfer
- [ ] Compliance requirements
- [ ] Inbound Data Transfer
- [ ] Licensing

**Explanation:**
The primary cost drivers for the campaign are Storage, Compute, and Outbound Data Transfer.

### 15)
You are a system administrator tasked with maintaining and managing a fleet of EC2 instances with AWS Systems Manager in your organization's AWS environment. You want to utilize a feature that allows you to group and visualize EC2 instances based on different criteria like applications, environment, or Region to simplify management and identify issues quickly.

**Which AWS Systems Manager feature would you primarily use to group and visualize your EC2 instances based on different criteria such as applications, environment, or Region?**
- [ ] Run Command
- [x] Resource Groups
- [ ] Parameter Store
- [ ] Maintenance Windows

**Explanation:**
Resource Groups in AWS Systems Manager allows you to group and visualize EC2 instances based on different criteria for efficient management.

### 16)
An organization wants a multi-AZ, highly durable, and scalable object storage solution to store Amazon EC2 instance data backups. Cost is not a concern. Primarily, they want the data to be quickly and easily restored in the event of an instance failure.

**Which AWS service would be MOST efficient to accomplish this task?**
- [ ] Amazon Elastic Block Store (EBS)
- [ ] Amazon Glacier
- [x] Amazon S3
- [ ] Instance Store

**Explanation:**
Amazon S3 provides highly durable, scalable, and efficient object storage suitable for storing EC2 instance data backups.

### 17)
A company must migrate an SAP HANA workload from on-premises servers to AWS.

**Which Amazon EC2 instances can be used?**
- [ ] Choose from the list of certified Amazon EC2 instances for SAP HANA workloads
- [ ] Choose Amazon EC2 instances from the P family
- [ ] Choose Amazon EC2 instances from the M family
- [x] Choose Amazon EC2 instances from the C family

**Explanation:**
For SAP HANA workloads, Amazon EC2 instances from the C family are recommended. 
