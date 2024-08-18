# Automation-of-EBS-Volumes-Type-Conversion
Type Conversion of EBS Volumes : gp2 to gp3


### PROJECT DESCRIPTION :

It is the responsibility of the Cloud Engineer to take care of the AWS Environment and make sure it is in compliance with the organizational policies.

AWS CloudWatch is used in combination with AWS Lambda to govern the resources according to the compliance policies of the organization.

A Lambda Function is triggered when an Amazon Elastic Block Store (EBS) Volume is created.

CloudWatch Events is used to monitor and respond to the EBS Volumes that are of type gp2 and convert them into type gp3.


### PROJECT WORKFLOW :

### Defining the Lambda Function :






Python script, designed for an AWS Lambda function, modifies the type of an Amazon EBS volume to 'gp3'. 

The get_volume_id_from_arn function extracts the volume ID from the provided Amazon Resource Name (ARN) by splitting the ARN string. 

In the lambda_handler function, the volume ARN is obtained from the event, and the volume ID is extracted using the get_volume_id_from_arn function. 

The boto3 library's EC2 client is then used to call modify_volume, which updates the volume type to 'gp3'. 

This function is triggered by an event containing the ARN of the EBS volume to be modified.









