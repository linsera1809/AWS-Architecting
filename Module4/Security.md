# Security

## RDS Security
* Access to the DB itself
    * Access control.
* Encryption at rest
    * Data is encrypted in the instance, it's backups, and it's replicas
* Encryption in transit
    * Encryption in transit with SSL
* Event notifications
    * Receive notifications for events
    * *NOTE: Create a CloudTrail to log this*

## DynamoDB
* Definable access permissions
* Encryption at rest
    * Offers fully managed encryption at rest
* SSL/TLS
    * Uses HTTPS by default