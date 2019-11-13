# Amazon RDS

## Scaling Vertical
* Aurora 1st Gen, MySQL, Postgres
    * Read-Replicas
        * Can create up to 15 Read-Replicas
        * Aurora Serverless does this for you
* Microsoft SQL and Oracle
    * Stop, lift, and shift
    
## DB Storage
* 16TB Volumes - Everything else
* 64TB Volumes - Aurora

## With Aurora:
* You can grow to 64TBs __in 10GB increments__
* You will have 6-replicas across 3-AZs
* Requires very little change to your existing application