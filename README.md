# Lambda

Given a Lambda function that is triggered upon the creation of files in an S3 bucket, answer the following:

1. What is the purpose of the execution role on the Lambda function?
- The purpose of the execution role is to grant the function access to AWS services and resources.

2. What is the purpose of the resource-based policy on the Lambda function?
- The purpose of the resource-based policy is to give other accounts or AWS resources permissions to invoke the Lambda function.

3. If the function is needed to upload a file into an S3 bucket, describe (i.e no need for the actual policies)
   - What is the needed update on the execution role?
     We need to ensure that we include a s3:PutObject action in the execution role

   - What is the new resource-based policy that needs to be added (if any)?
     No resource-based policy needs to be added

