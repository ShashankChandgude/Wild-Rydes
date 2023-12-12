## Setup

### AWS Account

In order to complete this project, I used a free tier AWS account and access to
create AWS Identity and Access Management (IAM), Amazon Cognito, AWS Lambda,
Amazon S3, Amazon API Gateway, AWS Amplify Console, Amazon DynamoDB, and AWS 
Cloud9 resources within that account.

As I was working on this project alone, code and instructions are modeled assung only one person is following and using AWS Account to complete this project.

Use a personal account or create a new AWS free tier account for this workshop.
Also ensure you do not leave behind any resources from the workshop as it might cause unintended billing.

### AWS Cloud9 IDE

Q. What is AWS Cloud9?
- AWS Cloud9 is a cloud-based integrated development environment (IDE) that lets
you write, run, and debug your code with just a browser. It includes a code
editor, debugger, and terminal. Cloud9 comes pre-packaged with essential tools
for popular programming languages and the AWS Command Line Interface (CLI)
pre-installed so you don’t need to install files or configure your laptop for
this workshop. Your Cloud9 environment will have access to the same AWS
resources as the user with which you logged into the AWS Management Console.



**Following are the Step-by-step Instructions**

1. Go to the AWS Management Console, click **Services** then select **Cloud9**
   under Developer Tools.

1. Click **Create environment**.

1. Enter `Development` into **Name** and write a short description **Description**.

1. Click **Next step**.

1. Leave **Environment settings** at their defaults of launching a new
   **t2.micro** EC2 instance.

1. Click **Next step**.

1. Review the environment settings and click **Create environment**.

1. Now IDE opens to a welcome screen. Below that, a terminal prompt is opened.

    Us this to run AWS CLI commands.
    Verify that login is succesfull by running `aws sts get-caller-identity`.

    ```console
    aws sts get-caller-identity
    ```

    A output indicating account and user information is showcased as following this output has detail specific to the user:

    ```console
    ec2-user:~/environment $ aws sts get-caller-identity
    ```
    ```json
    {
        "Account": "123456789012",
        "UserId": "AKIAI44QH8DHBEXAMPLE",
        "Arn": "arn:aws:iam::123456789012:user/Alice"
    }
    ```

As AWS Cloud9 IDE is essential it is best to keep it opened in a tab until you complete all the steps.

I havd kept an open scratch pad in Cloud9 for notes.  This is useful to note something such as
an ID or Amazon Resource Name (ARN), copy and paste that into the scratch pad.


### Next

Lets delv in first module, [Static Web Hosting][static-web-hosting], 
wherein I have deployed a static web site via AWS Amplify Console.

[region-table]: https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services/
[static-web-hosting]: ../1_StaticWebHosting/
