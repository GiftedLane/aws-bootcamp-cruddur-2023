# Week 0 — Billing and Architecture
## GitHub
> **get·hub** :   _a web-based platform for version control and collaborative software development_

-  ♾️ STEP 1 > [What is GitHub?](https://github.com/)
-  ♾️ STEP 2 > Clone the repo from [ExamProCo/aws-bootcamp-cruddur-2023](https://github.com/ExamProCo/aws-bootcamp-cruddur-2023) 
## Gitpod
> **get·pod** :   _a cloud-based integrated development environment (IDE)_

-  ♾️ STEP 1 > [What is Gitpod?](https://www.gitpod.io/about)
-  ♾️ STEP 2 > Change Gitpod to Darkmode
-  ♾️ STEP 3 > Create a new Gipod workspace for [GiftedLane/aws-bootcamp-cruddur-2023](https://github.com/GiftedLane/aws-bootcamp-cruddur-2023)
-  ♾️ STEP 4 > [403 error when pushing to my GitHub repo](https://github.com/gitpod-io/gitpod/issues/1315)

    _I did [a Google search](https://github.com/gitpod-io/gitpod/issues/1315) to find a fix for the issue. I had to set my Gitpod permissions to allow write access to my GitHub repo_ 😁
    <p align="left">
 <img src="img/gitpod-denied.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>
    <p align="left">
 <img src="img/gitpod-perms.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

## AWS
> **A·W·S** :   _the world's most comprehensive and broadly adopted cloud platform_

-  ♾️ STEP 1 > [What is AWS?](https://aws.amazon.com/what-is-aws/)
-  ♾️ STEP 2 > Enable MFA for AWS Root account and IAM User
    <p align="left">
 <img src="img/mfa-enabled.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

-  ♾️ STEP 3 > Login to my existing AWS account
-  ♾️ STEP 4 > Verify my billing alarms are in place for actual spend & credits spend

    _I created a monthly budget to alert me when my forcasted costs reaches 50% of $10. I created a second monthly budget for when my forecasted costs reaches 50% of $5._ 😁
    <p align="left">
 <img src="img/monthlyBillingBudget.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>
    <p align="left">
 <img src="img/monthlyBillingBudgetDetails2.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>
    <p align="left">
 <img src="img/credit-budget.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

-  ♾️ STEP 5 > Verify Admin User is created
    <p align="left">
 <img src="img/iam-admin-user.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

-  ♾️ STEP 6 > Generate AWS Credentials
    <p align="left">
 <img src="img/access-keys.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

-  ♾️ STEP 7 > Use CloudShell
    <p align="left">
 <img src="img/cloudshell.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

-  ♾️ STEP 8 > Install AWS CLI via Gitpod

    _I use the instructions via [the AWS site] (https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html#getting-started-install-instructions). I ran into trouble when I accidentally left the 'p' off the awscliv2.zip file._

    <p align="left">
 <img src="img/install-aws-cli.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>
    <p align="left">
 <img src="img/awscli-installed.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

# Lucidcart
-  ♾️ STEP 1 > [Create the Logical diagram](https://lucid.app/documents/view/c5ca0c98-9f6a-4324-95b8-ff77b68e12d5)
    <p align="left">
 <img src="img/Cruddur.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

-  ♾️ STEP  > Create the Concept Napkin diagram
    <p align="left">
 <img src="img/napkin.jpg?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

# Homework Challenges
> **fun** :   _how did you go beyond the class instructions_

## Destroy your root account credentials, Set MFA, IAM role
-  ♾️ STEP 1 > Destroy your root account credentials
    <p align="left">
 <img src="img/destroyKey.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>
    <p align="left">
 <img src="img/destroyKey2.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>
-  ♾️ STEP 2 > Enable MFA for AWS Root account and IAM User
    <p align="left">
 <img src="img/mfa-enabled.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

## Use EventBridge to hookup Health Dashboard to SNS
-  ♾️ STEP 1 > [What is EventBridge](https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html)
-  ♾️ STEP 2 > [New EventBridge – Track and Respond to Changes to Your AWS Resources](https://aws.amazon.com/blogs/aws/new-cloudwatch-events-track-and-respond-to-changes-to-your-aws-resources/)
-  ♾️ STEP 3 > [Creating an EventBridge rule for AWS Health](https://docs.aws.amazon.com/health/latest/ug/cloudwatch-events-health.html)

## Setup a Billing Alarm with SNS via the AWS CLI
-  ♾️ STEP 1 > [Create a topic](https://docs.aws.amazon.com/cli/latest/userguide/cli-services-sns.html)
-  ♾️ STEP 2 > [Subscribe to a topic](https://docs.aws.amazon.com/cli/latest/userguide/cli-services-sns.html#cli-subscribe-sns-topic)
-  ♾️ STEP 3 > Verify the alarm was created in AWS after confirmation email
    <p align="left">
 <img src="img/bill-alarm-cli.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>
    <p align="left">
 <img src="img/bill-alarm-cli2.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>

## Well-Architected Tool
-  ♾️ STEP 1 > Go through ALL the questions
-  ♾️ STEP 2 > Review the results
    <p align="left">
 <img src="img/welArchRisk.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>
    <p align="left">
 <img src="img/welArchRisk2.png?raw=true" alt="GIFTED LANE Logo" width="80%" height="80%" />
</p>