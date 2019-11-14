# Architecting on AWS 
__Bobby Linse__  
__11/12 to 11/14__

## Links:
* [Google Doc](https://tinyurl.com/AWSArchAssoc)
* [Books](https://evantage.gilmoreglobal.com/#/)
* [Exit Certified Labs](https://exitcertified.qwiklabs.com/)

## Contact:
* Instructor: Ruben Lopez
* [Email Support](mailto:imvp@exitcertified.com)

## Table of Contents:
* #### [Module 1: Introduction](/Module1)
    * [Intro](/Module1/Intro.md)
    * [The Well Architected Framework](/Module1/The-Well-Architected-Framework.md)
    * [AWS Global Infrastructure](/Module1/AWS-Global-Infrastructure.md)
    * [Large Scale Architectural Diagramming](/Module1/Large-Scale-Architectural-Diagram.md)
* #### [Module 2: The Simplest Architectures](/Module2)
    * [Intro to S3](/Module2/Intro-to-S3.md)
    * [Access Control](/Module2/Access-Control.md)
    * [Multipart Upload](/Module2/Multipart-Upload.md)
    * [S3 Costs](/Module2/S3-Costs.md)
    * [When Should You Use S3](/Module2/When-Should-You-Use-S3.md)
* #### [Module 3: Adding a Compute Layer](/Module3)
    * [Intro to EC2](/Module3/Intro-to-EC2.md)
    * [EC2 Pricing](/Module3/EC2-Pricing.md)
* #### [Module 4: Adding a Database Layer](/Module4)
    * [Intro to the Database Layer](/Module4/Intro-to-Database-Layer.md)
    * [DynamoDB](/Module4/DynamoDB.md)
    * [Amazon RDS](/Module4/Amazon-RDS.md)
    * [DB Migrations](/Module4/AWS-DB-Migrations.md)
    * [Security](/Module4/Security.md)
* #### [Module 5: Networking in AWS - Pt. 1](/Module5)
    * [Introduction to VPCs](/Module5/VPC-Intro.md)
    * [Routing](/Module5/Routing.md)
    * [Security in the Cloud](/Module5/Security-in-the-cloud.md)
* #### [Module 6: Networking in AWS - Pt. 2](/Module6)
    * [Introduction to Data Migration](/Module6/Intro.md)
    * [Load Balancers](/Module6/Load-Balancers.md)
* #### [Module 7: Identity and Access Management (IAM)](/Module7)
    * [Introduction to IAM](/Module7/Intro.md)
    * [Multiple Accounts](/Module7/Multiple-Accounts.md)
    * [Organizing My Users](/Module7/Organizing-my-Users.md)
* #### [Module 8: Elasticity, High Availability, and Monitoring](/Module8)
    * [Elasticity, High Availability, & Monitoring](/Module8/Intro.md)
* #### [Module 9: Automation](/Module9)
    * [Introduction to Cloud Automation](/Module9/Intro.md)
    * [CloudFormation Automation](/Module9/CloudFormation.md)
    * [Other Automation Tools](/Module9/AutoTools.md)
* #### [Module 11: Building Decoupled Architectures](/Module11)
    * [Introduction to Decoupling](/Module11/Intro.md)
    * [Simple Queue Service](/Module11/SimpleQueueService.md)
* #### [Module 12: Microservices and Serverless Architectures](/Module12)
    * [Introduction to Microservices and Serverless Architectures](/Module12/Intro.md)
    * [Container Services](/Module12/Container-Services.md)
    * [Going Serverless with Lambda](/Module12/Going-Serverless.md)

## Labs
1. __Lab 1:__ Hosting a Static Website
    * Create an S3 bucket and upload a static app to that bucket.
    * [Working Directory](/Lab1)
2. __Lab 2:__ Deploying a Web Application on AWS
    * Using EC2 and User Data to deploy and instantiate an instance.
3. __Lab 3:__ Creating a Virtual Private Cloud
    * Create an application with a VPC with a public and a private subnet that connects to an RDS instance and an EC2.
4. __Lab 4:__ Creating a Highly Available Environment
    * Create an auto scaling group, and a load balancer. 
    * Complete a multi-AZ deployment.
5. __Lab 5:__ Automating Infrastructure Deployment with AWS CloudFormation
    * Use CloudFormation to deploy a network, an application, and the Template Designer
    * [Working Directory](/Lab5)
6. __Lab 6:__ Implementing a Serverless Architecture with AWS Managed Services
    * Use Lambda, SNS, DynamoDB, and S3 to create an eCommerce site that displays inventory
    * [Working Directory](/Lab6)

## Resources:
* ### Case Studies
    * [S3 Breach: Republican National Convention](https://www.upguard.com/breaches/the-rnc-files)
    * [S3 Breach: Capital One](https://blog.cloudsploit.com/a-technical-analysis-of-the-capital-one-hack-a9b43d7c8aea)
* ### Automation Resource
    * [Pipelines: Github Actions with AWS](https://github.com/actions/aws/tree/master/cli)
    * [Pipelines:Configuring your Workflow](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/configuring-a-workflow#adding-a-workflow-status-badge-to-your-repository)
    * [Site Reliability: Chaos Monkey and the Simian Army](https://medium.com/netflix-techblog/the-netflix-simian-army-16e57fbab116)
    * [Sample CloudFormation Templates](https://aws.amazon.com/cloudformation/resources/templates/)
* ### Test Prep
    * [Exam Guide](ExamGuide.md)
    * #### Whitepapers
        * [Well Architected Framework](https://d1.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf)
    * #### FAQs
        * [Simple Queue Service](https://aws.amazon.com/sqs/faqs/)
        * [Relational Database Service](https://aws.amazon.com/rds/faqs/)
        * [Route 53](https://aws.amazon.com/route53/faqs/)
        * [VPC](https://aws.amazon.com/vpc/faqs/)
        * [S3](https://aws.amazon.com/s3/faqs/)
        * [EC2](https://aws.amazon.com/ec2/faqs/)
    * #### Practice Exams
        * [AWS Architecture 2019 - Kindle](https://www.amazon.com/Certified-Solutions-Architect-Practice-Questions-ebook/dp/B07BJGXPXK)