# Intro to S3

* How many servers do you get with an S3 bucket? __SIX__
* 4 - 9's __available__
* 11 - 9's __durable__
* S3 buckets are __scoped to the region__
* You get charged for GETting data from S3 buckets, but __Cloud Front Distribution__ (a cloudfront cache server) __is free when placed in front of your bucket__.
 

## Amazon S3
* Object-level storage
* Event triggers
    * __SQS__ - simple queueing service: manages all of the Event Triggers.
    * __SNS__ - simple notification service: making your triggers a subscribing-based model that applications can subscribe to.
    * __Lambda__ - serverless function that most triggers will be integrated with.
* Designed for 11 - 9's durablity (99.999999999999%)
    * Your responsibilities in maintaining 11 - 9s
        * Maintain your permissions
        * Object-locking
        * Version control 


