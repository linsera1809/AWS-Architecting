# AWS Database Migration

## AWS DMS (DB Migration Service)
* Supports migration to and from most commercial and open source database
* Can be used to migrate between dbs on EC2, RDS, and on-premise

## Migration Options
* One-time migration
* Ongoing migration
    * Installing the migration agent onto the physical service

## Snowball Edge with DMS
* Migrating data is unfeasible
    * Database is too large
    * Connection issues
    * Privacy and security concerns
* __USE SNOWBALL EDGE__

## AWS Schema Conversion Tool
* A standalone application that enables you to convert your existing db schema from 1 db engine to another  
![](aws-schema-conversion.PNG)