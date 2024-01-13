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
