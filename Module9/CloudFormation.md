# Cloud Formation

## AWS CloudFormation
* Provides a common language to describe your AWS infrastructure
* Creates and builds those described resources in an automated manner
* Templates:
    * A parameterized file that describes and defines the resources to be deployed in an environment
    * Either in JSON or in YAML
    * Put these in a code repository
* Allows _Drift Detection_ which will notify when the build has had an unexpected output

## Conditions of CloudFormation
* _Deleting the STACK of CloudFormation deletes all of the products of the stack_
* Your production and development environment __MUST__ be built from the same stack. 
    * This ensures that your application works in production the way it was designed and developed

## Making Changes
#### This is the basic workflow for using change sets:
* 1. Create a change set by submitting changes for the stack that you want to update. 
* 2. View the change set to see which stack settings and resources will change. 
* 3. If you want to consider other changes before you decide which changes to make, create additional change sets.
* 4. Execute the change set. AWS CloudFormation updates your stack with those changes.