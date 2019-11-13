# DynamoDB

## Intro
* Serverless non-relational database service
* Event-driven programming
* Extreme horizontal scaling capability
    * *Recommendation: Turn on auto-scaling with this*
* Transactions provide ACID across one or more tables within a __single AWS account and region__

## Works Well for:
* Have simple high-volume data 
* Need to scale quickly and with ease
* Don't need complex joins

## Issues with:
* Consistency
    * Eventual Consistent Reads
        * __Uses 0.5 RCUs__
    * Can upgrade to Strongly Consistent Reads
        * At a cost of performance
        * __At a cost of 1 RCU__

## DynamoDB
* Anything outside of a Partition key or Sort key scan, a Table scan will be performed.
    * To get around this, create a local index

## Credits
* 1 Read-Credit-Unit (RCU) = 4000 Bytes: Read per second
    * Enable credit-sharing for evenly distributed RCUs
* 1 Write-Credit-Unit (WCU) = 1000 Bytes: Write per second
* Partial credits are possible
    * e.g. If I use 3000 Bytes for a Read, there is still 1000 Bytes available in my RCU.

## Global Table Replication
* Allows for table replication across Regions
    * Synchronization is possible when enabling "Replication Stream"
* Multiplies the READS and the WRITES for each replica
    * i.e. This costs more credits