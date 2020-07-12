# SAM-BinaryAlert (BETA)

SAM-BinaryAlert can deploy BinaryAlert with SAR and SAM CLI. \
With SAR you can deploy with just a few clicks.(Required param is **NamePrefix** only) 

[BinaryAlert](http://www.binaryalert.io/) is a serverless, real-time framework for detecting malicious files. (Use cool Terraform) 

\* http://www.binaryalert.io/ \
\* https://github.com/airbnb/binaryalert \
\* SAM is Serverless Application Model\
\* SAR is Serverless Application Repogitory

## BinaryAlert vs SAM-BinaryAlert

|  | BinaryAlert | SAM-BinaryAlert |
| --- | --- | --- |
| Feature | Perfect | Simple, Convenient |
| How to deploy | Terraform | SAM, SAR |
| Functionality | Full | Almost the same.Currently not compatible with Carbon Black |
| Maintainability | Full | The core Lambda application is the same and always up to date (not forking). The infrastructure has been rewritten with the SAM Template. (I will do my best to catch up) |
| Limit | No limit | Each value that needs to be calculated requires parameter setting. Minutes have been changed to seconds, threshold parameters etc. are increasing. (cfn cannot be calculated!) |

## Deployment
There are two types of deployment procedures, SAR and SAM CLI.\
This section describes the procedure using SAM CLI.\
Click here for explanation of SAR.

## Deploy by SAR

1. AWS Web Console Login.
2. SAR [SAM-BinaryAlert](https://console.aws.amazon.com/lambda/home#/create/app?applicationId=arn:aws:serverlessrepo:ap-northeast-1:909044525866:applications/SAM-BinaryAlert) Jump.
3. Set a unique value for the **NamePrefix** parameter. (^[a-z][a-z0-9-_]{3,50}$)
4. Check to I acknowledge that this app creates custom IAM roles and resource policies.
5. Hit the deploy button. 

## Deploy by SAM CLI

Go to GitHub https://github.com/komikoni/sam-binaryalert#readme
