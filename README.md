# AWS 3-Tier-Web-Application
Multi-tier Architecture for a web application,used for high availability and scalability.

This architecture provides a scalable, fault-tolerant solution with load balancing and automatic scaling at each tier. The separation into different tiers allows for better management, scalability, and maintenance of the application.The Nginx server serves the static content to the React.js website and redirecting API calls is a common practice, and the combination of Node.js for the application logic and Aurora MySQL for the database further enhances the overall robustness of the system.

Parts Overview

Part 1 - Security and Networking
Establish the VPC and configure networking components for a secure and isolated environment.
Define security groups to control inbound and outbound traffic for EC2 instances, Aurora databases, and Elastic Load Balancers.

Part 2 - Database Deployment
Deploy the Aurora MySQL multi-AZ database and configure it for high availability.
Implement necessary security measures to protect the database layer.

Part 3 - App Tier Instance Deployment
Create an EC2 instance for the application tier.
Configure the instance to run a Node.js application on port 4000 and establish access to databases.

Part 4 - Internal Load Balancing and Auto Scaling
Create an AMI of the app tier instance.
Set up autoscaling with a load balancer to achieve high availability for the application tier.

Part 5 - Web Tier Instance Deployment
Deploy an EC2 instance for the web tier.
Configure the NGINX web server and deploy the React.js website.

Part 6 - External Load Balancer and Auto Scaling
Create an AMI of the web tier instance.
Set up autoscaling with an external-facing load balancer to enhance availability for the web tier.
