# Observability, monitoring and troubleshooting EC2

## Amazon EC2 Instance Status Checks

Which of the Amazon EC2 instance status checks require manual administrator intervention to resolve the issue?

- [ ] System status checks
- [x] Instance status checks
- [ ] Neither require manual intervention.
- [ ] Both checks require manual intervention.

#### Explanation

Instance status checks monitor the software and network configuration of your individual instance, detecting problems that require your involvement to repair. System status checks monitor the AWS systems on which your instance runs and detect underlying problems that require AWS involvement to repair.

---

## Amazon EC2 Metrics in Instance Dashboard

Which Amazon EC2 metrics can you view in the instance dashboard on the Amazon EC2 console? (Select THREE.)

- [x] CPU utilization
- [ ] RAM
- [x] Disk I/O
- [x] Network utilization
- [ ] Memory used
- [ ] Instance process ID

#### Explanation

You can monitor CPU utilization, disk I/O, and network utilization for your EC2 instances in the instance dashboard on the Amazon EC2 console. These metrics help you optimize and manage the performance of your instances.


## Amazon CloudWatch Metric Definition

In Amazon CloudWatch, a metric is defined as _______ and _________. (Select TWO.)

- [x] a time-ordered set of data points
- [ ] an object within a bucket
- [x] a resource to monitor
- [ ] the length of time that CloudWatch is running
- [ ] a date-severity set of data points

#### Explanation

A metric represents a time-ordered set of data points that are published to CloudWatch, making it a time-ordered set of data points. It is associated with a specific AWS resource, making it a resource to monitor.

---

## Amazon CloudWatch Agent Data Collection

The Amazon CloudWatch agent must be used to collect which type of data?

- [ ] CPU metrics
- [ ] Network utilization metrics
- [x] Host-level metrics
- [ ] Disk performance metrics

#### Explanation

To collect host-level metrics and logs, the CloudWatch agent must be installed. This is necessary to capture additional internal system metrics, such as memory utilization, that are not sent to the CloudWatch service by default.


## AWS Trusted Advisor Data Source

What gathered data does AWS Trusted Advisor provide its recommendations from? (Select TWO.)

- [x] AWS best practices
- [ ] Information gathered in user forums
- [x] AWS operational experience
- [ ] Data collected in customer surveys
- [ ] AWS tool feedback questionnaires

#### Explanation

AWS Trusted Advisor provides recommendations based on AWS best practices and operational experience gained from serving hundreds of thousands of AWS customers. It does not rely on user forums, customer surveys, or tool feedback questionnaires.


## Creating CloudTrail Trail with AWS CLI

Which option can you perform by using AWS CLI to create a trail?

- [ ] Create an all-Regions trail.
- [x] Create a single-Region trail.
- [ ] Create both a single-Region and all-Regions trail.
- [ ] You cannot create a trail from the AWS CLI.

#### Explanation

You can create a single-Region trail using the AWS CLI. The option to create an all-Regions trail is not available.

---

## Managing All-Regions Trail with New Region

What happens to your existing all-Regions trail if you add a new Region to your environment?

- [ ] A new single Region trail must be created.
- [ ] The new Region must be manually added to the existing trail.
- [x] The new Region is automatically added to the trail.
- [ ] You must delete and recreate the all-Regions trail.

#### Explanation

If a Region is added after you create an all-Regions trail, the new Region is automatically included in the trail, and events in that Region are logged. There is no need to manually add the new Region or delete and recreate the all-Regions trail.


## Troubleshooting SSH Connection Issues on Amazon EC2

As an AWS administrator for your company, you get a call stating that users cannot connect by using Secure Shell (SSH) to an Amazon EC2 instance in your main Region. You attempt to connect by using SSH but are also unsuccessful. Which of the following would be valid next steps? (Select TWO.)

- [x] Try to connect using the EC2 serial console.
- [ ] Build another EC2 instance and connect to it by using SSH.
- [ ] Check AWS Identity and Access Management (IAM) roles assigned to the instance.
- [x] Check the AWS Health Dashboard.
- [ ] Verify the instance can be restarted.

#### Explanation

1. **Try to connect using the EC2 serial console:**
   - Connecting to the EC2 serial console would be a valid next step to determine if the local console is still accessible, similar to plugging in a direct keyboard and monitor.

2. **Check the AWS Health Dashboard:**
   - Checking the AWS Health Dashboard would be a valid step to determine if there are any interruptions in AWS services that could prevent a successful SSH connection.

Building another EC2 instance and checking IAM roles are not immediate steps to troubleshoot the issue in this scenario. Restarting the instance might be considered after identifying the problem.

## Valid Approaches to Observability Strategy

Which of the following are valid approaches to an observability strategy? (Select TWO.)

- [ ] Step-by-step
- [x] Outside-in
- [ ] Big-picture
- [x] Inside-out
- [ ] Bi-directional

#### Explanation

1. **Outside-in:**
   - With an outside-in approach, you can analyze workload performance in the context of customer experience.

2. **Inside-out:**
   - With the inside-out approach, your observability strategy focuses on the health of your instance.

Step-by-step and big-picture approaches are not typically associated with observability strategies. Bi-directional is not a common term used in this context.

## Amazon CloudWatch Data Collection Periods

Which of the following statements is true for data collection periods for basic and detailed monitoring for Amazon CloudWatch metrics?

- [ ] Basic monitoring collects data in 5-second periods, and detailed monitoring collects data in 1-second periods.
- [ ] Basic and detailed monitoring use the same collection periods, but detailed monitoring provides more dimensions.
- [x] Detailed monitoring collects data in 1-minute periods, and basic monitoring collects data in 5-minute periods.
- [ ] Basic and detailed monitoring use the same collection periods, but detailed monitoring charges for data storage for extra dimensions.

#### Explanation

- Basic monitoring for EC2 instances is collected in 5-minute periods.
- Detailed monitoring collects data in 1-minute periods.
- The dimensions are the same for both monitoring options, but you are charged per metric that is sent to CloudWatch.

## Amazon EC2 Automated Status Checks

Amazon EC2 performs automated checks on every running EC2 instance to identify hardware and software issues. Which of the following statements are true for Amazon EC2 automated status checks? (Select TWO.)

- [ ] System status checks determine the health of the operating system in the EC2 instance.
- [x] System status checks determine if the AWS systems hosting the EC2 instance are healthy.
- [ ] Instance status checks determine if the AWS systems hosting the EC2 instance are healthy.
- [x] Instance status checks monitor the software and network configuration of your individual instance.
- [ ] System status checks determine the health of the network connectivity of your individual instance.

#### Explanation

- **System status checks:**
   - These checks determine if the AWS systems hosting the EC2 instance are healthy.

- **Instance status checks:**
   - These checks monitor the software and network configuration of your individual instance. They include checks such as checking the operating system's reachability and the status of the instance's network connectivity.

Other options are incorrect in describing the purpose of system and instance status checks.

## Connecting to Amazon EC2 Serial Console

What is required to connect to the Amazon EC2 serial console using a remote SSH client?

- [ ] It's a one-step process. Just change the SSH target to the syntax of `INSTANCE_ID.port0@serial-console.ec2-instance-connect.us-east-1.aws`.
- [x] 1 - Get the public key from the private key.
      2 - Push the SSH public key to the instance using the AWS CLI.
      3 - Use the private key with the SSH client to connect using the syntax of `INSTANCE_ID.port0@serial-console.ec2-instance-connect.us-east-1.aws`.
- [ ] 1 - Get the public key from the private key.
      2 - Push the SSH private key to the instance using the AWS CLI.
      3 - Use the public key with the SSH client to connect using the syntax of `INSTANCE_ID.port0@serial-console.ec2-instance-connect.us-east-1.aws`.
- [ ] You cannot use an SSH client to connect to the EC2 serial console. The browser-based EC2 serial console is the only way to make a serial connection to the EC2 instance.

#### Explanation

```
A connection to the EC2 serial console can also be established for an SSH client using the following process:

Get the public key from the private key (PEM file):
 ssh-keygen -y -f myprivate-key.pem > mypublic-key.pub
Push the SSH public key to the instance: 
aws ec2-instance-connect send-serial-console-ssh-public-key --instance-id i-0faeINSTANCE_ID --serial-port 0 --ssh-public-key file://mypublic-key.pub
Connect using a SSH client:
ssh -i  myprivate-key.pem INSTANCE_ID.port0@serial-console.ec2-instance-connect.us-east-1.aws(opens in a new tab)
See Connect to the EC2 Serial Console (opens in a new tab)for additional information.
```
