# Intro to EC2

## Things to Consider:
1. Frequency of Use
2. Instance Type
    * Components
        * Component Names:
            * Memory
            * CPU
            * Network Adaptors
            * Storage
        * These components are grouped together as a family, and then a class, and then a generation, and then the size
            * This is called the MODEL.
            * i.e. __COMPONENTS => FAMILY => CLASS => GENERATION => SIZE => MODEL__ 

## Virtual Machines vs. Physical Servers
* When using disposable resources
    * Data-driven decisions
    * Quick iterations
    * Free to make mistakes

## Amazon EC2s and AMIs
* AMI: A template for the root volume.
    * __Scoped for the REGION__
    * Launch permissions
    * AMIs are tied to the Amazon Kernal Image (AKI)
* EC2 Service will always create an image ID associated with your AMI
* Fully-Baked: an AMI template that is ready to be reused and pre-built. 
    * To make updates to certain pieces of the AMI you'll need to rebake the app
        * To get around this, you'd build a hybrid AMI.
* After the image is baked, a script is ran that is configuring the server. __This is called BOOTSTRAPPING.__ 

## Where To Get AMIs
* There are a few ways to get your AMI
1. Pre-Built
    * Ubuntu
    * Redhat
    * Amazon Linux
    * SUUS
    * Windows
2. Marketplace
    * Multi-ODM (verified vendors)
    * ~5,000 images, some with licenses included
3. Create your own
4. Community
    * __AWS DOES NOT SUPPORT THIS.__ But there are approx. 50,000 images.

## Launching EC2 Instances with User Data
* Your AMI
    * PENDING > RUNNING
        * Your OS is running and available in Pending
        * Running => Your USER DATA (i.e. your boot scripts) has completed configuring the servers.

## Retrieving Metadata
* http://169.254.169.254/latest/meta-data/public-hostname 
* In this url, it is getting meta data about the instance itself. 
* For example:
    * It may need to learn and share the public IP address 

## Amazon Elastic Block Store (EBS)
* Application needs __block level storage__
* Instance storage is __ephemeral__
* Needs data to persist through shutdowns
* Need to be able to back-up data volumes
* *NOTE: 30,000 Simultaneous Reads and Writes are possible with this*
* __IDEAL FOR:__
    * Temporary storage of frequently changing data
    * Caches
    * Buffers
    * Temporary Content
    * Data Replication for a Load-Balanced Pool

## EBS Volume Types
* Volume Types:
    * Solid-States
        * General Purpose SSD (GP2)
            * General purpose volume that balances price and performance
            * 1-16TB
            * 100-10K I/O per seconds
            * 250mB
            * __Best for Most Workloads__
        * Provisioned IOPS (IO1)
            * Highest-performance SSD volume for mission-critical low-latency
            * __Best for Critical Business Apps and Large DB workloads__
    * Hard-Disk Backed
        * Throughput Optimized HDD
            * Low cost HDD volume designed for frequently accessed, throughput-intensive workloads
            * __Best for Streaming, Data warehouses, Log processing__
            * __Cannot be a boot volume__
        * Cold HDD
            * Low cost HDD volume designed for less frequently access workloads
            * __Best for Throuput-oriented storage for large volumes of data that is INFREQUENTLY accessed__
            * Scenarios where lowest cost storage is important

## Amazon EBS
* An Amazon EBS–optimized instance uses an optimized configuration stack and provides additional, dedicated capacity for Amazon EBS I/O. 
* This optimization provides the best performance for your EBS volumes by minimizing contention between Amazon EBS I/O and other traffic from your instance.            

## Amazon Instance Networking
* Anytime AWS gives you LOW, MEDIUM, HIGH
    * ENI - Elastic Networking Interface
* Anytime AWS gives you 10, 20, 25
    * ENA - Elastic Networking Adaptor
* Anytime AWS gives you 50, 75, 100
    * EFA - Elastic Fabric Adaptor

### Honorable Mention - T Class
* Burstable Instance
    * Gives you a percentage of an overall CPU
    * Requires CPU credits per hour to acheive 100% credits

### Honorable Mention - Tagging
* EC2
    * 50 Tags per resource
* S3 
    * 50,000 tag limit