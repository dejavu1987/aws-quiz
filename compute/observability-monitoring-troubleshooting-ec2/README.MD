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
