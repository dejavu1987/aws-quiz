# EC2 Fundamentals

## Question 1: Instance Naming and Meanings

What does the letter 'g' mean in the instance name c6gn.xlarge?

- [ ] Instance family
- [ ] Generation
- [x] AWS Graviton processor
- [ ] Gigabyte

#### Explanation

Instance names can include additional capabilities. In this case:
- 'g' stands for AWS Graviton processors.

---

## Question 2: Choosing Instance Type for a Stateless Application

You have a stateless application that can recover when interrupted. Which instance type would you choose?

- [ ] Reserved Instance
- [ ] Dedicated Host
- [x] Spot Instance
- [ ] On-Demand Instance

#### Explanation

Spot Instances are useful for short workloads and workloads that can handle interruptions.

---

## Question 3: Advice on Changing to the Newest Amazon EC2 Instance Type

What advice would you give someone about changing to the newest Amazon EC2 instance type? (Select THREE.)

- [x] Change if you want an instance that is optimized for a specific workload.
- [ ] Never change.
- [x] Change for better performance.
- [x] Change for greater cost efficiency.
- [ ] Only change in rare circumstances because AWS generally manages new instances for you.
- [ ] Use general-purpose instances to avoid changing.

#### Explanation

You can change your instance type for specific workload optimization, better performance, or greater cost efficiency.

---

## Question 4: Rightsizing EC2 Instances After Deployment

After deployment and determining workload requirements, what are the best options to rightsize your EC2 instance? (Select TWO)

- [ ] EC2 does not support after deployment rightsizing.
- [x] Launch a new instance and migrate your application to the new instance.
- [x] Stop the instance, change the instance type, and restart the same instance with the new instance type.
- [ ] You cannot run multiple, different instance types. They must all be the same instance type.
- [ ] Stop the instance, terminate the instance, choose another instance type, and then migrate your application.

#### Explanation

After deployment, you can resize your instance by launching a new one and migrating your application or by stopping the instance, changing its type, and restarting it. You are not locked into your initial decision.

