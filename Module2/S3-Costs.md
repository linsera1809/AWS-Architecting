# S3 Costs

## Pay Only for what you use
* GBs per month
* Transfer OUT to other regions or the internet
* PUT, COPY, POST, LIST, and GET requests

## What you DON'T pay for
* Transfer IN
* Transfer OUT to EC2 in the same region or to CloudFront

## Tiering Models - Storage
* S3 Standard
* S3 Intelligent-Tiering (S3 INT)
* S3 Standard - Infrequent Access
    * Infrequent Access = 30 Days
* S3 One Zone - Infrequent Access
* S3 Glacier
    * Not being used for 60 Days
* S3 Glacier Deep Archive
    * 7 years or more
    * This is essentially a vault
        * Set your permissions restrictively
        * Once vault lock is enabled, va

## Data Restore Options
* Expedited Restore:  1 to 5 minutes
* Standard Restore: 3 - 5 hours
* Bulk Restore: 5 - 12 hours
* Glacier Deep Restore: 12 - 48 hours

## Lifecycle Policies
* Allows you to delete or move objects based on age
* Example:
    * Dont use something for 30 days?
        * It will be moved into an S3 Infrequent Access
            * Dont use something for 60 days? 
                * Moved to Glacier
