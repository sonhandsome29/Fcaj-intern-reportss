---
title : "Clean up"
date : 2026-07-10
weight : 9
chapter : false
pre : " <b> 5.9. </b> "
---

#### Clean up resources

After finishing the Project Management deployment workshop, you should remove the AWS resources to avoid unnecessary charges. The sequence below is arranged to reduce dependency errors while deleting the environment.

#### Recommended order

1. **Remove the frontend deployment on AWS Amplify**

   Open **AWS Amplify** and select the deployed app. If you no longer need the demo environment, delete the active branch or remove the entire hosting app.

2. **Delete the Amazon Cognito configuration**

   In **Amazon Cognito**, review and remove:

   - The User Pool created for this project
   - The related App Client
   - Any test users that are no longer needed

3. **Delete the API in Amazon API Gateway**

   Open **API Gateway** and remove:

   - The HTTP API or REST API created for the project
   - The deployed stage
   - Any authorizer created specifically for the lab

4. **Delete the Lambda trigger**

   If you created a Lambda function for post-confirmation or another Cognito trigger:

   - Detach the trigger from the User Pool
   - Delete the Lambda function if it is no longer required

5. **Stop and terminate the EC2 backend**

   In **EC2 Console**:

   - Stop the instance for a final check
   - Terminate the backend instance when you are done
   - Release any Elastic IP that was attached
   - Delete the key pair on AWS if you do not need it anymore

6. **Delete the Amazon RDS database**

   In **RDS Console**, decide whether you want to keep a final snapshot:

   - Keep a snapshot if you may need the data later
   - Skip the snapshot if this was only a lab environment

   Then delete the database instance.

7. **Delete the S3 bucket used for images**

   In **Amazon S3**:

   - Delete all objects inside the bucket
   - Confirm that the bucket is empty
   - Delete the bucket used for project images or static assets

8. **Delete security groups and supporting network resources**

   After EC2 and RDS are removed, you can delete:

   - The EC2 security group
   - The RDS security group
   - The DB subnet group if it was created specifically for this workshop

9. **Delete the subnets, route tables, internet gateway, and VPC**

   If the VPC was created only for this workshop, remove it in this order:

   - Subnets
   - Custom route tables
   - Internet gateway (detach first, then delete)
   - VPC

#### Final note

Before deleting everything, make sure you have already saved:

- The final source code
- Screenshots used in the report
- Any important configuration values or demo links you may need later
