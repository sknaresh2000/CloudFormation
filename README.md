# CloudFormation
*This repo contains cloudformation templates and can be used for learning cloudformation*
### 01-Basic FullStack Template
This template creates the below resources and uses CloudFormation-Init and UserData
- Autoscaling group with Launch Configuration
- Application Load Balancer with Target Group
- Security Group for EC2 to allow incoming connections from Application Load Balancer
- Security Group for ELB allowing connections from the world

### 02-LAMP Stack Template
This template creates the below resources with Creation, Deletion Policy along with cfn-hup to detect and update the instances by running user specific actions
- EC2 Instance along with wordpress configuration
- RDS Instance
