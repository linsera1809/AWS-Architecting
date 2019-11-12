## What is the cloud? What is AWS?
* Programmable Resources
* Dynamic abilities
* Pay as you go

* What other advantages does the cloud offer?
    * Global infrastructure as a service
    * Maintenance
    * Differentiated heavy lifting
        * What does that mean? This is the day-to-day infrastructure support
            * e.g. Server patching, rack maintenance, security

* Does this mean that there are no responsibilities of the customer?
    * No. This is the concept of the shared responsibilities model. 
        * Some responsibilities include:
            * Security
            * Scaling
            * Load balancing 

### Programmable Resources
* CloudFormation
    * Building full stacks programmatically based on a created template
* OpsWorks
    * Similar to Chef and Puppet (This is a Selenium-like automation tool)
* BeanStalk
    * Fullstack pipelining tool that auto-provisions instances/resources 

### Dynamic Abilities
* Auto-Scaling
* Load-Balancing
* Lambda Functions `Technically... this is based on event-triggers but it is still dynamic`

### Pay As You Go

* No need to buy hardware or build data centers
    * Pay as you consume resources
    * Reduce upfront capital costs
        * `NOTE: There is a link to Ruben's infrastructure calculator [here](https://docs.google.com/document/d/1Du1zDz2ZXC6e9VjN1PmdKFwQ5rIvp9BPyKrGwcjV3Sg/edit)`

#### Cost Explorer
*  Not extremely user-friendly, but it is very customizable  
*  Using Tags makes the ability to search, pair instances into resource groups, and filter your resources

#### The Scale Advantage
__Leverage large economies of scale.__
* Lower cost than on your own
    * Specialized hardware and software
    * Large volume hardware purchasing

__Some Notes__
    * `AWS owns 80% of the world's storage`
    * `Their power comes directly from the power companies directly to the Data Centers`
    * `Every cable to/from their data centers`

#### The Capacity Advantage
* Stop guessing about capacity
    * Scale up and down as needed
        * __VERTICAL SCALING__: Creating larger instances
        * __HORIZONTAL SCALING__: Creating more instances 

#### The Speed Advantage
* No need to wait for hardware
    * New IT resources are just a click away
    * Reduce resource development time.

#### The Focus Advantage
* Focus on your applications, not your infrastructure.
    * Free up resources to spend on new projects
    * Stop spending money running and maintaining data centers
    * Disposable resources allow for quick experimentation

#### The Global Advantage 
* Go global in minutes
    * Multiple AWS Regions around the world
    * Keep your application close to your users
    * Facilitate high availability and disaster recovery

##### CloudFront
* Content Delivery Network
    * A distribution that defines your origin server
    * Caches content and delivers to the customers as needed
    * `NOTE: Every 100 milliseconds of latency lost in AWS equates to a 1% loss of their global customers`
