# AWS Three Tier Web Architecture Workshop

## Description
This workshop is a hands-on guide to building a three-tier web system in AWS. We'll create the necessary network, security, application, and database components step by step, making it available and scalable.

## Audience
This workshop is for beginners with a technical background. We assume you have some basic knowledge of AWS services like VPC, EC2, RDS, S3, ELB, and the AWS Console.

## Prerequisites
1. An AWS account. If you don't have one, follow the instructions [here](https://aws.amazon.com/console/) and click "Create an AWS Account" in the top right corner to set it up.
2. Any code editor of your choice.

## Architecture Overview
![Architecture Diagram](https://github.com/aws-samples/aws-three-tier-web-architecture-workshop/blob/main/application-code/web-tier/src/assets/3TierArch.png)

In this setup, a public-facing Application Load Balancer directs user traffic to our web servers. The web servers use Nginx to host a React.js website and pass API requests to an internal-facing load balancer. This internal load balancer forwards the requests to the application tier, written in Node.js. The application tier interacts with an Aurora MySQL database to retrieve and manipulate data. We've set up load balancing, health checks, and auto-scaling to ensure the system's availability.

## Workshop Instructions
You can follow the step-by-step instructions in the [AWS Three Tier Web Architecture Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/85cd2bb2-7f79-4e96-bdee-8078e469752a/en-US).

## Security
For information on reporting security issues, refer to [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications).

## License
This library is licensed under the MIT-0 License. For details, see the LICENSE file.
