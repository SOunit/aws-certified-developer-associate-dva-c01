# steps

- check

  - no EC2 instance is running
  - load balancer is shot down
  - no auto-scaling-group available

# create elastic beanstalk application

- name application
- no tag, skip tag
- select platform
  - node.js
- select sample application
- create

# what is created?

- go to events in ElasticBeanstalk
- create
  - environment
  - AWS S3
  - target group
  - application load balancer
  - security group
  - auto scaling group
