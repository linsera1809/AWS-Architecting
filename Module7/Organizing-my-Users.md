# Organizing My Users

## IAM User Groups
* Using User Groups make permissions user agnostic
* Example:
    * New hire joins Developers group.
    * New hire leaves Developers group and their access.
    * New hire joins Testing group 
    * New hire joins Testing group and their access.

## Need a Temporary User?
* Use IAM Roles
    * A role lets you define a set of permissions to access the resources that a user or service needs
    * The permissions are not attached to an IAM user or group
    * The permissions are attached to a role and the role is assumed by the user or the service
    * Should be used temporarily

## IAM Roles
* Use Cases
    * Provide AWS resources with access to AWS services
    * Provide access to externally authenticated users
    * Provide access to third parties
    * Switch roles to access resources in:
        * Your AWS account
        * Any other AWS account (cross account access)
    