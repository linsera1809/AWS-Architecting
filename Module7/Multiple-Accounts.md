# Multiple Accounts

## AWS - In the Wild
* How many accounts do you need?
* Examples:
    * One Account
        * Create multiple VPCs
    * Multiple Accounts
        * Split your environments up into multiple accounts 
            * Prod
            * Staging
            * Test
            * Dev

## How do I manage all of these account?
* AWS Organizations
    * Centralized account management
        * Group based account management
        * Policy based access to AWS services
            * Service-Control Policies
        * Automated account creation and management
        * Consolidated billing
        * API-based
    * Two way to deploy this:
        1. Using it just for consolidated billing
        2. Using it for every Organizational Units (OU)

## If I create an Admin:
* The admin was just granted Allow to everything..
* What can't they do?
    * Delete the account
    * Consolidated Billing
    * Personal Data