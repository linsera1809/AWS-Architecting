# Load Balancers

## Elastic Load Balancing
* A Managed load balancing service that distributes incoming application traffic across multiple Amazon EC2 instances, containers, and IP addresses
* Load Balancers are scoped to the VPC
* __Application Load Balancing__ -- HTTP/HTTPS
    * These are usually your EXTERNAL load balancers 
* __Network Load Balancing__ -- SSL/TCP
* __Classic Load Balancer__ -- Provides basic load balancing across EC2 instances in Multi-AZ and operates at both the request level
    * This is being depricated
* Each load balancer is given a DNS Name
* As soon as you register your application, the ELB will attempt to recognize & respond to __unhealthy instances__

## Why should you use ELB
* High availability
    * Multi-AZ deployments
* Health checks
* Security features
    * Leverage its network scurity features by default.
* TLS termination

## Application Load Balancing
* Comes with a Content AND a Path load balancer.
* Options are available for content load balancing
    * __ECS__ -- Elastic Container Services
    * __EKS__ -- Elastic Kubernetes Services
    * __Fargate__ -- Platform agnostic service for connecting ECS and EKS