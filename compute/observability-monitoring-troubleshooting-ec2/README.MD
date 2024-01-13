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
