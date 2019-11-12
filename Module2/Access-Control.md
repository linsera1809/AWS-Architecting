# Access Control

* Permissions are regulated on the bucket level __AND__ the object level.
* __By default, every permission is Private__
* Any object in a READ-ONLY bucket, is set to READ-ONLY
* The better way to implement this is using CONTROLLED access.

## Bucket Policies
* [Policy Generator Resource](https://awspolicygen.s3.amazonaws.com/policygen.html)
* Principal Entitities
    * Users
    * Groups
    * Roles

## Amazon Resource Names
* arn:partition:service:region:account-id:resource
* arn:partition:service:region:account-id:resourcetype/resource
* arn:partition:service:region:account-id:resourcetype:resource

* Examples:
    * arn:aws:cloudtrail:us-east-1:123456789012:trail/mytrailname
    * arn:aws:s3:::williewonka/photos/penguins.jpg
        * *Note: Some services are GLOBAL and because of this, Regions and Account-ID are NULL*

* [Resource Names](http://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html)

## Versioning
* __By default versioning is turned off.__
* Inherent benefits:
    * You can't overwrite your data
    * 11 - 9's durability
    * Deleted items can be easily restored
* Deleted objects are just hidden from view with delete markers
* S3-Intelligent Tiering is the most efficient method of managing/space within versioning

## Access Control - CORS
* Cross-Origin Resource Sharing - defines a way for client web apps that are loaded in one domain to interact with resources in a different domain

## S3 for Data Computation 
* EMR (Elastic Map Reduce) - used for Hadoop clusters
    * Serverless Batch Database
* Kinesis - real-time analytics and media transcoding
* Redshift - relational database / datawarehouse analytics tool
* Quicksight - Visualization & Dashboarding tool

## S3 for Backup Tools
* Want to Back up?
* 2 Options:
    * Using VPN
    * Direct Connect
        * 1GB or 10GB connections
* Used to make that connection:
    * Storage Gateway
        * Install the agent on the Data Center server
        * 3 Options
            1. Volume Gateway
                * Presents a volume or another drive on the server
                * You can include adding a cache option if you'd like to optimize costs from Data Center to object.
            2. File Gateway: NFS Version for NAS (or SMB for Windows)
                * Making your S3 essentially a mounting location for data upload
                * *Note: Want data synchronization between the two for constant read/write?*
                    * Use DataSynch
            3. VTL (Virtual Tape Library)
                * An automated tape organization solution for storage
    