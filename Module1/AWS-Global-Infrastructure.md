# AWS Global Infrastructure

## Data Centers
* A Single data center typically houses tens of thousands of servers
* All data centers are online, not "cold"
* AWS custom network equipment:
    * Multi-ODM sourced
        * In other words they are choosing the best vendor
            * `For example, they were using the ZEN hypervisor.. They are now using their own propriety.`
        * Customized network protocol stack

## AWS Availability Zones
* Each Availabilty Zone is:
    * Made up of __one or more__ data centers
    * Designed to be fault tolerant
    * Interconnected with other Availability Zones using high-speed PRIVATE links
    * You can choose your Availability Zone
    * AWS recommends replicating across AZs for resiliency

* Note: We seperate AZs by __FLOOD ZONES__ 

## AWS Regions
* Each AWS Region is made up of two or more Availability Zones.
    * AWS has 18 regions worldwide.
    * You enable and control data replication across regions.
    * Communication between regions uses AWS backbone network infrastructure.

    * Designing for High Availability
        * Elastic Load Balancing: Allows you to maintain the high availability accross multiple Availability Zones with load balancing.

    * Designing for Disaster tolerance: 
        * Deploy across multiple regions!

`NOTE: 60-65% of all data transfers happen in the DC area (N. Virginia)`

### There are 4 Architectural Considerations when choosing a REGION for deployment.
1. Performance: be closer to your customers.
    * If your customers are in South America, you wouldn't want to maybe have an Oregon deployment.

2. Costs of services. 
    * For all intents and purposes, services are scoped for that region. 
        * For example, Sao Paulo is double the cost for S3 buckets as opposed to Ohio.

3. Availability of Services.
    * Services are dependent on which area you are in.
        * For example: 'Alexa for Business' is __ONLY__ available in Northern Virginia.

4. Compliance.
    * For example If you are a Government based entity, you are required to use GOV-Cloud-West 

`NOTE: Everything is an API call, everything else is a permission`

### Edge Locations
1. Route53
2. CloudFront
3. IAM
4. Web-Application Firewall (WAF)
5. Shield
    * You can upgrade your service to Advanced Shield which will give you WAF for free.