
**AWS SAA-C02 Study Guide**

This study guide will help you pass the newer AWS Certified Solutions Architect - Associate exam. Ideally, you should reference this guide while working through the following material:

1.  Stephane Maarek's [Ultimate AWS Certified Solutions Architect Associate 2021 course](https://links.datacumulus.com/aws-certified-sa-associate-coupon) (permanent discount available through this link) or A Cloud Guru's [AWS Certified Solutions Architect Associate SAA-C02 course](https://acloud.guru/learn/aws-certified-solutions-architect-associate)
2.  The FAQs for the most critical services, included in the recommended reading list below
3.  Tutorials Dojo's [AWS Certified Solutions Architect Associate Practice Exams](https://www.udemy.com/course/aws-certified-solutions-architect-associate-amazon-practice-exams-saa-c02/)
4.  Andrew Brown's [AWS Certified Solutions Architect - Associate 2020 (PASS THE EXAM!) | Ad-Free Course](https://www.youtube.com/watch?v=Ia-UEYYR44s)

*Notes*: If at any point you find yourself feeling uncertain of your progress and in need of more time, you can postpone your AWS exam date. Be sure to also keep up with the ongoing discussions in [r/AWSCertifications](https://reddit.com/r/AWSCertifications/) as you will find relevant exam tips, studying material, and advice from other exam takers. Before experimenting with AWS, it's very important to be sure that you know what is [free](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc) and what isn't. Relevant Free Tier FAQs can be found [here](https://aws.amazon.com/free/free-tier-faqs/). Finally, Udemy often has their courses go on sale from time to time. It might be worth waiting to purchase either the Tutorial Dojo practice exam or Stephane Maarek's course depending on how urgently you need the content.

**Table of Contents**

1.  [Introduction](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#introduction)
2.  [Identity Access Management (IAM)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#identity-access-management-iam)
3.  [Simple Storage Service (S3)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#simple-storage-service-s3)
4.  [CloudFront](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#cloudfront)
5.  [Snowball](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#snowball)
6.  [Storage Gateway](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#storage-gateway)
7.  [Elastic Compute Cloud (EC2)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#elastic-compute-cloud-ec2)
8.  [Elastic Block Store (EBS)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#elastic-block-store-ebs)
9.  [Elastic Network Interfaces (ENI)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#elastic-network-interfaces-eni)
10. [Security Groups](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#security-groups)
11. [Web Application Firewall (WAF)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#web-application-firewall-waf)
12. [CloudWatch](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#cloudwatch)
13. [CloudTrail](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#cloudtrail)
14. [Elastic File System (EFS)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#elastic-file-system-efs)
15. [Amazon FSx for Windows](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#amazon-fsx-for-windows)
16. [Amazon FSx for Lustre](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#amazon-fsx-for-lustre)
17. [Relational Database Service (RDS)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#relational-database-service-rds)
18. [Aurora](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#aurora)
19. [DynamoDB](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#dynamodb)
20. [Redshift](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#redshift)
21. [ElastiCache](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#elasticache)
22. [Route53](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#route53)
23. [Elastic Load Balancers (ELB)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#elastic-load-balancers-elb)
24. [Auto Scaling](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#auto-scaling)
25. [Virtual Private Cloud (VPC)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#virtual-private-cloud-vpc)
26. [Simple Queuing Service (SQS)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#simple-queuing-service-sqs)
27. [Simple Workflow Service (SWF)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#simple-workflow-service-swf)
28. [Simple Notification Service (SNS)](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#simple-notification-service-sns)
29. [Kinesis](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#kinesis)
30. [Lambda](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#lambda)
31. [API Gateway](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#api-gateway)
32. [CloudFormation](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#cloudformation)
33. [ElasticBeanstalk](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#cloudformation)
34. [AWS Organizations](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#aws-organizations)
35. [Miscellaneous](https://github.com/surajsh999/AWS-SAA-C02-Study-Guide?search=1#miscellaneous)

**Introduction**

[**The official AWS Solutions Architect - Associate (SAA-C02) exam guide**](https://d1.awsstatic.com/training-and-certification/docs-sa-assoc/AWS-Certified-Solutions-Architect-Associate-Exam-Guide_v1.1_2019_08_27_FINAL.pdf)

**Exam Content Breakdown:**

[![Screen Shot 2020-06-05 at 2 49 08 PM](file:///C:/Users/WORKST~1/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)](https://user-images.githubusercontent.com/13093517/83912374-c2b87900-a73b-11ea-9691-b38383b43ff9.png)

*Domain 1: Design Resilient Architectures*

1.1 - Design a multi-tier architecture solution

1.2 - Design highly available and/or fault-tolerant architectures

1.3 - Design decoupling mechanisms using AWS services

1.4 - Choose appropriate resilient storage

*Domain 2: Design High-Performing Architectures*

2.1 - Identify elastic and scalable **compute** solutions for a workload

2.2 - Select high-performing and scalable **storage** solutions for a workload

2.3 - Select high-performing **networking** solutions for a workload

2.4 - Choose high-performing **database** solutions for a workload

*Domain 3: Design Secure Applications and Architectures*

3.1 - Design secure access to AWS resources

3.2 - Design secure application tiers

3.3 - Select appropriate data security options

*Domain 4: Design Cost-Optimized Architectures*

4.1 - Identify cost-effective **storage** solutions

4.2 - Identify cost-effective **compute** and **database** services

4.3 - Design cost-optimized **network** architectures

**Recommended Reading:**

You can cover a lot of ground by skimming over what you already know or what you can infer to be true. In particular, read the first sentence of each paragraph and if you have no uncertainty about what is being said in that sentence, move on to the first sentence of the next paragraph. Take notes whenever necessary.

1.  [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/wellarchitected-framework.pdf)
2.  [Amazon VPC FAQs](https://aws.amazon.com/vpc/faqs/)
3.  [AWS Autoscaling FAQs](https://aws.amazon.com/autoscaling/faqs/)
4.  [Amazon EC2 FAQs](https://aws.amazon.com/ec2/faqs/)
5.  [Amazon EC2 Auto Scaling FAQs](https://aws.amazon.com/ec2/autoscaling/faqs/)
6.  [Amazon EBS FAQs](https://aws.amazon.com/ebs/faqs/)
7.  [Elastic network interfaces](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-eni.html)
8.  [Amazon S3 FAQs](https://aws.amazon.com/s3/faqs/)
9.  [Elastic Load Balancing FAQs](https://aws.amazon.com/elasticloadbalancing/faqs/)
10. [Amazon Route 53 FAQs](https://aws.amazon.com/route53/faqs/)
11. [AWS Storage Gateway FAQs](https://aws.amazon.com/storagegateway/faqs/)
12. [Amazon EFS FAQs](https://aws.amazon.com/efs/faq/)
13. [Amazon FSx for Windows File Server FAQs](https://aws.amazon.com/fsx/windows/faqs/)
14. [Amazon FSx for Lustre FAQs](https://aws.amazon.com/fsx/lustre/faqs/)
15. [AWS Organizations FAQs](https://aws.amazon.com/organizations/faqs/)

**Identity Access Management (IAM)**

**IAM Simplified:**

IAM offers a centralized hub of control within AWS and integrates with all other AWS Services. IAM comes with the ability to share access at various levels of permission and it supports the ability to use identity federation (the process of delegating authentication to a trusted external party like Facebook or Google) for temporary or limited access. IAM comes with MFA support and allows you to set up custom password rotation policy across your entire organization. It is also PCI DSS compliant i.e. payment card industry data security standard. (passes government mandated credit card security regulations).

**IAM Entities:**

**Users** - any individual end user such as an employee, system architect, CTO, etc.

**Groups** - any collection of similar people with shared permissions such as system administrators, HR employees, finance teams, etc. Each user within their specified group will inherit the permissions set for the group.

**Roles** - any software service that needs to be granted permissions to do its job, e.g- AWS Lambda needing write permissions to S3 or a fleet of EC2 instances needing read permissions from a RDS MySQL database.

**Policies** - the documented rule sets that are applied to grant or limit access. In order for users, groups, or roles to properly set permissions, they use policies. Policies are written in JSON and you can either use custom policies for your specific needs or use the default policies set by AWS.

[![Screen Shot 2020-06-06 at 10 49 48 PM](file:///C:/Users/WORKST~1/AppData/Local/Temp/msohtmlclip1/01/clip_image003.png)](https://user-images.githubusercontent.com/13093517/83959193-11533980-a848-11ea-9d03-d8133e0aaa86.png)

IAM Policies are separated from the other entities above because they are not an IAM Identity. Instead, they are attached to IAM Identities so that the IAM Identity in question can perform its necessary function.

**IAM Key Details:**

-   IAM is a global AWS services that is not limited by regions. Any user, group, role or policy is accessible globally.
-   The root account with complete admin access is the account used to sign up for AWS. Therefore, the email address used to create the AWS account for use should probably be the official company email address.
-   New users have no permissions when their accounts are first created. This is a secure way of delegating access as permissions must be intentionally granted.
-   When joining the AWS ecosystem for the first time, new users are supplied an access key ID and a secret access key ID when you grant them programmatic access. These are created just once specifically for the new user to join, so if they are lost simply generate a new access key ID and a new secret access key ID. Access keys are only used for the AWS CLI and SDK so you cannot use them to access the console.
-   When creating your AWS account, you may have an existing identity provider internal to your company that offers Single Sign On (SSO). If this is the case, it is useful, efficient, and entirely possible to reuse your existing identities on AWS. To do this, you let an IAM role be assumed by one of the Active Directories. This is because the IAM ID Federation feature allows an external service to have the ability to assume an IAM role.
-   IAM Roles can be assigned to a service, such as an EC2 instance, prior to its first use/creation or after its been in used/created. You can change permissions as many times as you need. This can all be done by using both the AWS console and the AWS command line tools.
-   You cannot nest IAM Groups. Individual IAM users can belong to multiple groups, but creating subgroups so that one IAM Group is embedded inside of another IAM Group is not possible.
-   With IAM Policies, you can easily add tags that help define which resources are accessible by whom. These tags are then used to control access via a particular IAM policy. For example, production and development EC2 instances might be tagged as such. This would ensure that people who should only be able to access development instances cannot access production instances.

**Priority Levels in IAM:**

-   **Explicit Deny**: Denies access to a particular resource and this ruling cannot be overruled.
-   **Explicit Allow**: Allows access to a particular resource so long as there is not an associated Explicit Deny.
-   **Default Deny (or Implicit Deny)**: IAM identities start off with no resource access. Access instead must be granted.

**IAM Security Tools:**



