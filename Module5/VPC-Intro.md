# VPC Introduction

## Introduction to VPC Specifics
* VPC: Your private network space in the cloud
* Provides logical isolation for your workloads
* Allows custom access controls and security settings
* __VPCs are scoped to the REGION__
* Availability Zones are scoped to the VPC
* Subnets are scoped to the VPC

## Limits
* Soft limit: Default limits that can be raised
    * Allowed to create 5 VPCs per region
* Hard limit
    * 1 VPC cannot talk to more than 125 VPCs

## Use Case: Using One VPC
* *Placement Groups* are used in local VPC
    * Use dedicated host
    * Use singular AZ
* Small, single application
* High performing computions

## Use Case: Multi-VPC Pattern
* Single team or single orgs
* Maintains standards/permissions

## Use Case: Multi-Account Pattern
* Large organizations and organizations with multiple IT teams
* Medium-sized organizations that anticipate rapid growth