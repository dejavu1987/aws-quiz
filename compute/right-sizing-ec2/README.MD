## Turning on AWS Cost Explorer

With which of the following methods can you turn on AWS Cost Explorer?

- [ ] AWS Command Line Interface (AWS CLI)
- [ ] AWS API
- [x] AWS Management Console
- [ ] AWS Identity and Access Management (IAM) role

#### Explanation

Cost Explorer is turned on through the AWS Management Console. At this time, there is no option to turn on Cost Explorer through the API.

## Historical Data in AWS Cost Explorer

How many months of historical data can you view using AWS Cost Explorer?

- [ ] 3
- [ ] 6
- [ ] 9
- [x] 12

#### Explanation

You can view the previous 12 months of your data and can forecast the next 12 months of possible future spending.

## Exploring Costs in AWS

With which tool can you explore costs BEFORE you incur them?

- [ ] AWS Cost Explorer
- [x] AWS Budgets
- [ ] AWS Cost and Usage Reports
- [ ] AWS Trusted Advisor

#### Explanation

AWS Budgets is a cost planning and forecasting tool before expenses show up. It is designed to proactively alert you if your cost or usage goes up. Cost Explorer creates reports to help you analyze cost and usage data after you have incurred the cost. It also provides historical data and recommendations on what you can do to lower costs in the future.

## Historical Usage Data for AWS Budgets

How many weeks of historical usage data is needed by AWS Budgets before it can begin to generate a budget forecast?

- [ ] 1
- [ ] 3
- [x] 5
- [ ] 7

#### Explanation

Note that AWS requires approximately 5 weeks of usage data to generate budget forecasts. If you set a budget to alert based on a forecasted amount, this budget alert isn't initiated until you have enough historical usage information.

## Modifying an EC2 Instance

To modify an instance, you must know what resources the instance has. What is the term for the combined virtual hardware components of an instance?

- [ ] Instance family
- [x] Instance type
- [ ] Instance generation
- [ ] Instance

#### Explanation

An instance type is the combination of virtual hardware components, such as CPU and memory, that make up the instance. EC2 instances are sized based on the combined hardware resources consumed by that instance type. This means the size is the total configured capacity of vCPU, memory, storage, and networking. This is important information to have if you need to change the size or type of your instance.

## AWS Nitro System Innovation

Which innovation helps the AWS Nitro System improve instance performance?

- [ ] Offloading the hypervisor to memory
- [x] Using dedicated hardware to offload I/O operations
- [ ] Adding more powerful solid-state drives (SSDs) for data
- [ ] Offloading I/O to host-attached disk drives

#### Explanation

The Nitro System is a combination of dedicated hardware and a lightweight hypervisor, for faster innovation and enhanced security. The most beneficial part of the Nitro System hardware is that it uses dedicated hardware to offload I/O operations.

## Inhibitors to Changing Instance Type

If an instance type cannot be changed, what options might be inhibiting your ability to change the instance type? (Select TWO.)

- [ ] The instance type is newer than the one currently running.
- [x] Hibernation is enabled on the instance.
- [x] The instance is a Spot Instance.
- [ ] The instance is stopped.
- [ ] The EBS volume is not attached.

#### Explanation

You cannot change the instance type if hibernation is enabled. A Spot Instance cannot be changed to an instance of another type.

---

## Importance of Network Interfaces in Rightsizing

True or false? The number of network interfaces needed by an instance is an important consideration when rightsizing EC2 instances.

- [x] True
- [ ] False

#### Explanation

The number of network interfaces needed by an instance is an important consideration when rightsizing EC2 instances. This is because the number of network interfaces available in EC2 is type specific. For example, a t2.micro instance type allows for a maximum of two network interfaces, while a trn1.32xlarge supports up to eight network interfaces.

## Compatibility Factors in Changing Instance Type

In a rightsizing project, it is determined that the price performance could be improved if current t2.medium x86_64 instances were changed to c6g.large 64-bit Arm Graviton instances to support enhanced networking. What compatibility factors should be considered? (Choose TWO.)

- [x] A new Amazon Machine Image (AMI) will need to be selected for the new instance type, and then the data will need to be migrated.
- [ ] The new instance type will not require a new Amazon Machine Image (AMI). The instance just needs to be shut down to change the instance type.
- [x] The paravirtual (PV) virtualization type will change because the new instance will be a hardware virtual machine (HVM) on the Nitro hypervisor.
- [ ] The virtualization type does not matter because all instance types run on all AWS-supported hypervisors.

#### Explanation

Changing the instance type from x86_64 to Arm Graviton may require a new AMI, and data migration might be necessary. Additionally, the virtualization type may change from paravirtual (PV) to hardware virtual machine (HVM) on the Nitro hypervisor.

## Steps for Changing Instance in an Instance Store-Backed EC2 Instance

When running an instance store-backed EC2 instance, which steps must you take to use a different instance? (Select THREE)

- [x] Create an Amazon Machine Image (AMI) from your existing image.
- [ ] Create a new EC2 instance.
- [x] Launch a new instance with the (AMI).
- [x] Migrate your applications.
- [ ] No need to migrate. The applications will still be there.
- [ ] Back up the data in the instance store.

#### Explanation

To use a different instance in an instance store-backed EC2 instance, you need to create an AMI from your existing image, launch a new instance from this AMI, select the instance type that you want, and then migrate your application to the new instance.

## Changing Instance Type for Workload Optimization

What options do you have if you have chosen an instance type that appears to be the wrong fit for your workload? (Select TWO.)

- [x] Switch the existing instance type to a new one.
- [x] Launch a new instance and migrate your application to the new instance.
- [ ] Stop the instance, change the type, and migrate the workload.
- [ ] Stop the instance, terminate the instance, choose another type, and then migrate your application.
- [ ] You cannot run multiple, different instance types. They must all be the same instance type.

#### Explanation

If you find that your chosen instance type is not suitable for your workload, you can either switch the existing instance type to a new one or launch a new instance with the desired type and migrate your application to the new instance. This allows you to optimize your workload based on changing requirements.

## Advice on Changing to the Newest Amazon EC2 Instance Type

What advice would you give someone about changing to the newest Amazon EC2 instance type? (Select THREE.)

- [x] Change if you want an instance that is optimized for a specific workload.
- [ ] Never change.
- [x] Change for better performance.
- [x] Change for greater cost efficiency.
- [ ] Only change in rare circumstances because AWS generally manages new instances for you.
- [ ] Use general-purpose instances to avoid changing.

#### Explanation

Changing to the newest Amazon EC2 instance type can be advisable if you want an instance optimized for a specific workload, if you seek better performance, or if you aim for greater cost efficiency. AWS regularly introduces new instance types with improvements, and selecting the right instance type based on your requirements can lead to enhanced performance and cost savings.

## Meaning of "g" in Instance Name c6g.large

What does the letter g mean in the instance name c6g.large?

- [ ] Instance family
- [x] AWS Graviton processor
- [ ] Gigabyte
- [ ] Generation

#### Explanation

In the instance name c6g.large, the letter "g" signifies that the instance is powered by AWS Graviton processors. Instance names can include additional capabilities, and the letter "g" specifically denotes the use of AWS Graviton processors.

## AWS Nitro System Functions Offloaded onto Hardware Cards

Which of the following functions did the AWS Nitro System offload onto hardware cards? (Select THREE.)

- [x] Virtual private cloud (VPC) networking
- [ ] Security groups
- [x] Instance storage
- [x] Amazon Elastic Block Store (Amazon EBS)
- [ ] Amazon Elastic File System (Amazon EFS)
- [ ] Amazon Simple Storage Service (Amazon S3)

#### Explanation

The AWS Nitro System offloads certain functions onto dedicated hardware cards for optimized performance:

- **Nitro Card for VPC Networking:**
  - Handles VPC data plan offload, including encapsulation, security groups, flow logs, routing, port mirroring, DNS, and DHCP.
  - Performs data-in-transit with no performance overhead to the host.
  - Offers an Elastic Network Adapter (ENA) and an Elastic Fabric Adapter (EFA).

- **Nitro Card for Amazon EBS:**
  - Supports storage acceleration for Amazon EBS.
  - Provides transparent encryption.
  - Monitors the SSD drives for wear.

- **Nitro Card for Instance Storage:**
  - Utilizes NVM Express (NVMe) for local instance storage.

## AWS Resource Tags

Which items make up a resource tag? (Select TWO.)

- [ ] Instance type
- [ ] Amazon Machine Image (AMI)
- [x] Key
- [x] Value
- [ ] Instance family

#### Explanation

A tag is a label that you assign to your resources, consisting of a key and an optional value:

- **Key:** A name for the tag, which is case-sensitive.
- **Value:** An optional, corresponding value for the tag.

## Instance Scaling

What happens to instances when they scale out?

- [ ] Larger instances are created.
- [x] Additional instances of the same type are created.
- [ ] Additional instances of a different type are created.
- [ ] Smaller instances are created.

#### Explanation

When scaling out, additional instances of the same type are created. This is typically done in response to increased demand to distribute the workload and maintain performance.

## Identifying Under-Utilized EC2 Instances

You are looking to downsize an instance. Which tool helps you identify only under-utilized EC2 instances?

- [ ] AWS Compute Optimizer
- [ ] AWS Cost and Usage Reports
- [x] AWS Cost Explorer
- [ ] AWS Budgets

#### Explanation

AWS Cost Explorer helps you identify under-utilized EC2 instances that can be downsized. This tool only shows downsizing information of your current instance to another instance in that same instance family. It also gives you detailed information on the potential impact to your costs by taking into account any of your Reserved Instances and instances in a Savings Plan.

## Identifying Downsizing and Upsizing Opportunities

Your instances are part of an Auto Scaling group. You need to identify opportunities to downsize and upsize these instances. Which tool helps you identify both downsizing and upsizing Amazon EC2 instances?

- [ ] Amazon CloudWatch
- [x] AWS Compute Optimizer
- [ ] AWS Trusted Advisor
- [ ] AWS Cost Explorer

#### Explanation

AWS Compute Optimizer provides recommendations for both downsizing and upsizing Amazon EC2 instances. It offers suggestions for instances that are part of an Auto Scaling group, helping you optimize your resources for better performance and cost efficiency.

## Changing Instance Type of EBS-Backed Instance

The following steps are used to change the instance type of an EBS-backed instance when the new instance type is compatible with the original instance type. Which is the correct order of the steps?

- [x] 1– Stop the instance; 2 – Select the new instance type; 3 – Install new drivers; 4 – Start the instance from the Amazon EC2 console.
- [ ] 1– Stop the instance; 2 – Select the new instance type; 3 – Start the instance from the Amazon EC2 console; 4 – Install new drivers.
- [ ] 1– Select the new instance type; 2 – Install new drivers; 3 – Stop the instance; 4 – Start the instance from the Amazon EC2 console.
- [ ] 1– Stop the instance; 2 – Select the new instance type; 3 – Install new drivers; 4 – Start the instance from the Amazon EC2 console.

#### Explanation

1. If the new instance type requires drivers that are not installed on the existing instance, you must connect to your instance and install drivers first (for example, when moving to an instance based on the AWS Nitro System).

2. Stop the instance from the Amazon EC2 console.

3. With the instance still selected, choose Actions, Instance settings, Change instance type, and select the new instance type. If the instance type you selected supports EBS optimization, select EBS optimized to enable EBS optimization.

4. Start the instance from the Amazon EC2 console.
