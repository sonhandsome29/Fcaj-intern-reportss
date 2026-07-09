---
title : "Clean up"
date : 2026-07-08
weight : 9
chapter : false
pre : " <b> 5.9. </b> "
---

#### Clean up resources

After finishing the **Project Management** deployment workshop, cleaning up the AWS resources is an important final step to avoid unnecessary costs. Because the services in this project depend on one another, the safest approach is to remove them from the outside in: start with the public-facing application components, then move back toward the backend, the database, and finally the networking layer. This makes the cleanup process smoother and reduces dependency-related errors.

#### Recommended order

1. **Remove the frontend deployment on AWS Amplify**

   First, open **AWS Amplify** and review the frontend application that was deployed for the project-management system. If the public demo is no longer needed, remove the active branch deployment or delete the hosting app entirely.

2. **Delete the Amazon Cognito configuration**

   Next, go to **Amazon Cognito** and review the authentication resources used by the project:

   - The User Pool created for this project
   - The related App Client
   - Any test users created during verification

3. **Delete the API in Amazon API Gateway**

   After that, open **API Gateway** and remove the public API layer used to expose the backend:

   - The HTTP API or REST API created for the project
   - The deployed stage
   - Any Cognito Authorizer created specifically for this system

4. **Delete the Lambda trigger**

   In this project, Lambda may be used for post-confirmation handling after user signup. Before deleting it, make sure to:

   - Detach the trigger from the User Pool
   - Review any remaining permissions or references
   - Delete the Lambda function if it is no longer required

5. **Stop and terminate the EC2 backend**

   Once the frontend and public access layer have been removed, go to **EC2 Console** and clean up the backend server:

   - Stop the instance for a final check
   - Terminate the backend instance when you are done
   - Release any Elastic IP that was attached
   - Delete the key pair on AWS if you do not need it anymore

6. **Delete the Amazon RDS database**

   For **Amazon RDS**, take a moment to decide whether the project data should be preserved before deletion:

   - Keep a final snapshot if you may need the data later for review or demonstration
   - Skip the snapshot if this was only a practice environment

   Once the appropriate option has been chosen, delete the database instance.

7. **Delete the S3 bucket used for images**

   In **Amazon S3**, remove the bucket used for project images or static files, such as `project-management-images-aws`, in this order:

   - Delete all objects inside the bucket
   - Confirm that the bucket is empty
   - Delete the bucket used for project images or static assets

8. **Delete security groups and supporting network resources**

   After EC2 and RDS have been removed, continue with the supporting network resources:

   - The EC2 security group
   - The RDS security group
   - The DB subnet group if it was created specifically for this workshop

9. **Delete the subnets, route tables, internet gateway, and VPC**

   Finally, if the VPC was created only for this project-management workshop, remove the network layer in the following order:

   - Subnets
   - Custom route tables
   - Internet gateway (detach first, then delete)
   - VPC

#### Final note

Before removing everything completely, make sure the following items have already been saved:

- The final source code
- Screenshots used in the report
- Any important configuration values, demo links, or sample environment settings you may need later
