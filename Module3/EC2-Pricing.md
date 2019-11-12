# EC2 Pricing Options

## On-Demand Instances
* Linux and Ubuntu
    * By the second
* Windows 
    * By the hour

## Reserved Instances
* 75% discount on instances
* Define the instance
    * A little difficult because you need to know what instance you need
* Define the term
    * Reserve for 1 to 3 years
    * Partial upfront (PU)
    * No upfront (NU)
* Define the type
    * Convertable Instance
        * Stuck with the Class of your instance type
    * Standard Instance
        * Stuck with the instance type that you selected
* Sublease your reserved instances on the AWS Marketplace

## Spot Instances
* If you need something on-demand this is most cost-efficient way to do it.
* Name your price
* *Don't go too low, because if someone is willing to pay higher, AWS may terminate your instances*

## Dedicated Options
* Dedicated Instances
* Dedicated Hosts
    * "You want the full server"
    * Single Tenacity
    * You'll receive the HOST-ID
        * Makes you more compliant
        * Still comes with a Hypervisor
    * **Note: if you want a server without a hypervisor, get a Bare-Metal option. Warning.. this is expensive**
