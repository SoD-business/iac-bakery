# Gorgeous Cupcakes Infrastructure Setup

## Contents

- [Description for Developers](#developer-description)
- [Description for Non-Developers](#non-developer-description)

## Developer Description 👨‍💻

### Project Overview:

This AWS CloudFormation script sets up the necessary infrastructure for the Gorgeous Cupcakes web application. It defines parameters for a VPC, EC2 instances, Security Groups, an RDS database, and a Target Group for a Load Balancer.

### Technology Used

- AWS CloudFormation
- AWS EC2
- AWS RDS
- AWS VPC
- AWS Elastic Load Balancing (ELB)

### File Structure:

- `gc-dev-ec2.yml`: CloudFormation script to set up the Elastic Compute Cloud.
- `gc-dev-rds.yml`: CloudFormation script to set up the Relational Database Service.
- `gc-dev-vpc.yml`: CloudFormation script to set up the Virtual Private Cloud.

### Usage:

1. Ensure you have AWS CLI installed and configured with the necessary credentials.
2. Run the command `aws cloudformation create-stack --stack-name GorgeousCupcakesStack --template-body file://gorgeous-cupcakes-cf.yaml` in your terminal.
3. Monitor the AWS CloudFormation console for the status of your stack.

### Why was this created?

- To automate the provisioning and management of the infrastructure required for the Gorgeous Cupcakes application.
- To ensure infrastructure consistency, repeatability, and to follow infrastructure as code (IaC) best practices.

---

## Non-Developer Description 🙍‍♂️

### Project Overview:

This project sets up the technical foundation for our Gorgeous Cupcakes website to run smoothly on Amazon's cloud service. It specifies the necessary elements like servers, security settings, and database configuration.

### How it Works:

- This script is like a blueprint that tells Amazon's cloud service how to set up and connect the different technical parts needed for our website.
- Once run, it automatically creates and configures these parts according to the specified settings, ensuring our website has the resources it needs to operate.

### Why was this created?

- To simplify and speed up the setup process, ensuring everything is set up correctly and consistently, which helps in avoiding potential technical issues.
- It's a part of managing our website's technical setup in a modern and efficient way, ensuring it can handle our visitors reliably.
