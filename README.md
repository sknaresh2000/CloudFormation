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

### 03-BasicServicesTemplate
This contains the templates to create basic services which can be used along with other templates.
- S3 Bucket Creation
- User and IAM Roles

### 04-SaasModelTemplate
This contains the templates to create a basic SaaS model such as provision infratsruture and application depending upon the application version. 
- Infrastructure Setup(VPC, Internet Gateway, Public Subnets, NAT Gateways and configure Route Tables, S3 Bucket)
- Application Setup(Private, Public Subnets, Application load balancer with Target group, Auto scaling group with health check. This template is dependednt on the Infrastructure setup and so need to be imported only after the Infrastructure Setup template)
