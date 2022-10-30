# Typical architecture Web App 3-tier

- Public Subnet
  - Route53
  - ELB
    - Elastic Load Balancer
- Private Subnet
  - auto scaling group
- Data Subnet
  - Elastic Cache
  - Amazon RDS
    - read / write data

# developer problems on AWS

- managing infrastructure
- deploying code
- configure all the databases, load balancers, etc.
- scaling concerns

- most web apps has the same architecture(ALB + ASG)
  - ALB(Application Load Balancer)
  - ASG(Automatic Scaling Group)

# Elastic Beanstalk - overview

- developer centric view of deploying application on AWS
- uses all components
  - EC2 / Virtual Machine
  - ASG / Automatic Scaling Group
  - ELB / Elastic Load Balancer
  - RDS / Relational Database System
- manged service
  - automatically
    - handle capacity provisioning
    - load balancing
    - scaling
    - application health monitoring
    - instance configurations
  - just application code is responsible for developer
- we still have full control over configuration

# components

- application
  - collection of Elastic Beanstalk components(environments, versions, configurations)
- application version
- environment

  - collection of AWS resources running an application versions
  - Tiers
    - Web Server Environment Tier & Worker Environment Tier
  - You can create multiple environment

- summary

  - create application
  - upload version
  - launch environment
  - manage environment

- update
  - update version
  - upload version
  - launch environment
  - manage environment

# Web Server Tier vs. Worker Tier

-
