# Build with EC2

## Question 1: Security Features in Amazon EC2 Instances

Which security feature is connected to the elastic network interface of an Amazon EC2 instance and not at the subnet boundary?

- [ ] Access control list (ACL)
- [x] Security group
- [ ] Network access control list (network ACL)
- [ ] Internet gateway

#### Explanation

Security groups are attached to the elastic network interface of the AWS resources within the subnet.

---

## Question 2: Troubleshooting Outbound Traffic in Network ACLs

You have created an inbound network access control list (network ACL) rule allowing traffic from the internet into your web server. You are monitoring network traffic and you can see the traffic coming into the server, but no internet traffic is moving outbound. What should you do to resolve this?

- [ ] Create an outbound security group rule allowing traffic on port 80 out to the internet.
- [ ] Create an inbound network ACL allowing traffic on port 80 into the subnet.
- [ ] Add a new security group allowing port 80 into your web server from your database instance.
- [x] Create an outbound network ACL allowing traffic on port 80 to the internet.

#### Explanation

Network ACLs are stateless and require explicit rules for both inbound and outbound traffic.

---

## Question 3: Logical Data Centers Within a Region

What does AWS call logical data centers within a Region?

- [ ] Access zones
- [ ] Regional zones
- [ ] Virtual private clouds (VPCs)
- [x] Availability Zones

#### Explanation

An Availability Zone is a group of data centers within a Region.

---

## Question 4: Considerations for Data Placement

What are the considerations for determining where to place your data? (Select THREE.)

- [x] Compliance
- [ ] Currency types
- [x] Service availability
- [ ] Hardware offerings
- [x] Proximity to users
- [ ] Administrative proximity to the data center

#### Explanation

Considerations include compliance, service availability, and proximity to users.

---

## Question 5: Security Group Placement in AWS

A security group is a firewall that sits on which component?

- [ ] VPC
- [ ] Network
- [ ] Instance
- [ ] Availability Zone
- [x] Elastic network interface

#### Explanation

Security groups are attached to the elastic network interface of AWS resources within the subnet.

---

## Question 6: True Statements About Network Access Control Lists (Network ACLs)

Which of the following statements are true for network access control lists (network ACLs)? (Select THREE.)

- [ ] Network ACLs are stateful.
- [x] Network ACLs are stateless.
- [x] One-way routing rule
- [ ] Two-way routing rule
- [x] The default network ACL allows all inbound and outbound traffic.
- [ ] The default network ACL denies all inbound and outbound traffic.

#### Explanation

Network ACLs are stateless, operate with one-way routing rules, and the default network ACL allows all inbound and outbound traffic by default.
