# Connect to EC2 Quiz

## 1. Connecting to Large Organization's Location-Based IT Departments

Your organization is large and has many location-based IT departments. You do not want to share Secure Shell (SSH) key pairs with the various locations.

### Which connection option/s could you use?

- [ ] Connect by SSH
- [x] Amazon EC2 Instance Connect
- [x] AWS Systems Manager Session Manager
- [ ] Remote Desktop Protocol

**SUBMIT**

**Correct:**
Both AWS Systems Manager and EC2 Instance Connect provide a secure way to connect to your Linux instances without requiring key pairs. You use AWS Identity and Access Management (IAM) policies and principals to control SSH access to your instances. EC2 Instance Connect removes the need to share and manage SSH key pairs.

---

## 2. Administering Amazon EC2 Instances without Port 22

Your security department has rejected your requests to allow administrative traffic from your network to the AWS Cloud on port 22.

### Which option will allow you to administer your Amazon EC2 instances?

- [ ] Connect by Secure Shell (SSH)
- [ ] Amazon EC2 Instance Connect
- [x] AWS Systems Manager Session Manager
- [ ] Connect by PuTTY

**SUBMIT**

**Correct:**
With Session Manager, you can manage your Amazon EC2 instances through a browser-based shell or through the AWS Command Line Interface (AWS CLI). Session Manager removes the need to open inbound ports, manage SSH keys, or use bastion hosts.

---

## 3. Administering Amazon EC2 Linux Instance from Remote Hubs

You need to administer your Amazon EC2 Linux instance from one of your company's remote hubs. You have an internet connection and the key pairs for the instance.

### How should you connect?

- [x] Connect by Secure Shell (SSH)
- [ ] AWS Systems Manager Session Manager
- [ ] Remote Desktop Protocol
- [ ] Amazon EC2 Instance Connect

**SUBMIT**

**Correct:**
SSH authentication to an EC2 instance is done through the use of the key pair you associated with the instance when you launched it. The key pair makes it possible to secure, connect, and manage the instance. Losing the key pair can result in a loss of access to the instance.
