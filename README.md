# .Net Web Application
#### Deploy a .NET Web Application on Amazon ECS powered by Graviton2



This project consists of building a container image for an ASP.NET MVC 5 web application and deploy it onto an Amazon ECS cluster powered by Graviton2 instances. 

As part of this process, the AWS CLI will be use to create the container image for ARM architecture and push it to Amazon ECR which is a managed private repository service on AWS. Then to create a highly available Amazon ECS cluster with ARM based instances. Using AWS CloudFormation will launch a cluster of worker nodes on Amazon EC2, then launch a containerized Movie application onto your cluster. 


### What is Amazon ECS?

 Amazon ECS stands for Amazon Elastic Container Service, is a highly scalable, reliable, secure, fast container management service that makes it easy to run, stop, and manage containers on a cluster. without having to worry about running your own cluster management and container orchestration software. 
 
 Because ECS has been a foundational pillar for key Amazon services, it can natively integrate with other services such as Amazon Route 53, AWS Secrets Manager, AWS Identity and Access Management (IAM) and Amazon CloudWatch providing a familiar experience to deploy and scale containers. ECS is also able to quickly integrate with other AWS services to bring new capabilities to ECS.

AWS announced new EC2 instance types will be powered by the AWS Graviton2 processor. This processor is based on he ARM64 architecture leveraging 64-bit ARM Neoverse N1 cores; which make the Graviton2 instances about 20% less expensive per hour than Intel x86 instances with up to 40% better performance.


### Prerequisites

* AWS Account with administrator-level access.

* Recommended browser: he latest version of Chrome or Firefox 

* Foundational knowledge on AWS, CloudFormation, Docker and Linux 



#### Application Architecture
This project uses Amazon ECS, Amazon EC2 ARM based instance, and Elastic Load Balancing as pictured below:

![](pics/project-diagram.png)


