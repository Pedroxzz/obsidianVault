# CloudFront Foundation I
Welcome to the Amazon CloudFront Workshop.

In this workshop you will learn how to set up content delivery with CloudFront, and optimize performance of your application by using CloudFront.
### About the workshop

Each of the Chapters consist of a few sections that provide information about implementation steps for specific use cases. It will take approximately 90 minutes to complete the workshop from beginning to end.

Please remember to clean up the resources after the workshop to avoid any unnecessary costs.
### Target Audience

AWS Cloud Practitioners who would like to improve their knowledge of Amazon CloudFront through a series of hands-on excercises.

### Scenario

You are a solutions architect, and your objective is to build a CloudFront distribution that delivers an HTML website, an API, and video content. The origin is built on serverless architecture and consists of Amazon S3, Amazon API Gateway, AWS Lambda, and AWS Elemental MediaPackage.

In each section of the workshop you will face a challenge, and will use various features of CloudFront to solve it.
# Overview of CloudFront
Amazon CloudFront is a content delivery network (CDN) service built for high performance, security, and developer convenience.

Amazon CloudFront is a web service that speeds up distribution of your static and dynamic web content, such as .html, .css, .js, and image files, to your users. CloudFront delivers your content through a worldwide network of data centers called edge locations. When a user requests content that you're serving with CloudFront, the request is routed to the edge location that provides the lowest latency (time delay), so that content is delivered with the best possible performance.

If the content is already in the edge location with the lowest latency, CloudFront delivers it immediately.

If the content is not in that edge location, CloudFront retrieves it from an origin that you've defined—such as an Amazon S3 bucket, a MediaPackage channel, or an HTTP server (for example, a web server) that you have identified as the source for the definitive version of your content.

# Preparation

This workshop can be performed as part of an AWS Event or as a standalone excercise within an AWS Account. Please follow the preparation steps described in the appropriate section depending on which option you are following.
## AWS Event
If you are running this workshop during an AWS Event please ignore the **Using your account** section and follow the information from the expandable section below.

You start the lab with an already built website, API endpoint, and a media stream. In this lab, you'll login to the AWS account provided for this workshop, and verify the deployed web application.

### Step 1. Login into Workshop studio Event
To access the AWS account provided for this workshop, follow the instructions below.

1. You must obtain the sign-in URL from the event organizer. Connect to the event sign-in URL, and you will see below page. Click **Email One-Time Password (OTP)** button.
2. Enter your email address and click **Send passcode**.
3. Check the subject **Your one-time passcode** email in your email box.
4. Copy the passcode and paste it as shown below, then press the **Sign in** button.
5. You will see event access code, which is already fill-in. Click **Next**.
6. Check the checkbox **I agree with the Terms and Conditions** and click **Join event**.
7. In the left menu, click **Open AWS Console** button and the AWS Console will open in a new browser window.

### Step 2. Test your web application
#### Take Note of the cloudfront-workshop outputs in CloudFormation:

Go to the AWS Console, navigate to CloudFormation > Stacks > cloudfront-workshop and check the **Outputs** tab. Take note of the following Outputs:

- apiOriginEndpoint
- originBucket
- s3WebsiteDomain
- videoOriginDomain

#### Access the web application

Open up the web application in a browser window using the S3WebsiteDomain URL and verify that you see the following results:

## Using your own AWS account

If you are running this workshop in your own AWS account please ignore the **AWS Event** section and follow the information from the expandable section below.

You will spin up an already built website, an API endpoint, and a media stream. In this lab, you'll use a CloudFormation template to launch the web application.

### Step 1. Disable S3 Public Access

By Default AWS automatically blocks s3 Public Access requests to S3 buckets. For the start of this workshop you will need to disable this feature. We will re-enable this feature at a later time.

Navigate to the S3 Service within the AWS Console and select **Block Public Access settings for this account** in the left hand menu. Click Edit and Deselect the checkbox next to **Block _**all**_ public access** and click Save changes

### Step 2. Deploy the CloudFormation Stack

#### Download the CloudFormation template

```
curl 'https://static.us-east-1.prod.workshops.aws/f3c4f0f2-f631-4972-97ab-d50210825a95/static/cfn/cloudfront-workshop.yaml?Key-Pair-Id=K36Q2WVO3JP7QD&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9zdGF0aWMudXMtZWFzdC0xLnByb2Qud29ya3Nob3BzLmF3cy9mM2M0ZjBmMi1mNjMxLTQ5NzItOTdhYi1kNTAyMTA4MjVhOTUvKiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0MTM0ODUxOX19fV19&Signature=WTD4ne8DuBsmekzMp0CqGmjc5K889l-bw-A9RHi0Cm2bfeNQLQBQgS9viXwoFPWKOVZGJGpigUUzqJO3U30pdw0uoO8dPYUylY01Oxnqtje38TTczLv1BZt5RrpXN~O4K8XPnpMeycewQVibziXiL~tD0NSlHGqZ2JBtCgR3aCfhjE3z4QxQrZdOtnPqu0sUKqeF5iwJwEVkKj8Rh6w-B6UwJBC1hg4cGyCmb65Af3pZ9kO3dUFjendN2u3jNkb1nVAEeGs56r8AZ~pX6APeqHkwouFFGgFCk0fE2BrvleuP1l4l7l~uTLVukeJzmJfOzlTzDuiN9RyOU-xD-esOxA__' --output cloudfront-workshop.yaml
```

Launch the CloudFormation stack in **the us-east-1 N. Virginia Region**. The template will create the following resources:

- An API Gateway with Lambda functions
- IAM roles that Lambda functions will assume
- S3 buckets with web page
- MediaPackage for stream

The link will automatically bring you to the CloudFormation dashboard and start the stack creation process in the specified region. In **Template source,** choose _Upload a template file_ and upload the file you just download, enter _cloudfront-workshop_ as stack name, proceed through the wizard to launch the stack. Leave all options at their default values, but make sure to check the box to allow CloudFormation to create IAM roles on your behalf:

Name your stack cloudfront-workshop and put **content-acceleration-cloudfront-workshop-aws-asset** as **AssetsBucketName** parameter name. Leave the **AssetsBucketPrefix** blank

Click Next
Keep all of the defaults **Configure stack options** menu
Click Next
Accept the Acknowlegment that AWS CloudFormation might create IAM resources

After you click on **Submit**, and please wait for the stack to show **CREATE_COMPLETE** in green under status, it takes about 3 minutes for the stack to be created.

### Step 3. Test your web application
#### Take Note of the cloudfront-workshop outputs in CloudFormation:
Go to the AWS Console, navigate to CloudFormation > Stacks > cloudfront-workshop and check the **Outputs** tab. Take note of the following Outputs:

- apiOriginEndpoint
- originBucket
- s3WebsiteDomain
- videoOriginDomain
#### Access the web application
Open up the web application in a browser window using the S3WebsiteDomain URL and verify that you see the following results:

# CloudFront basic configuration
In this section you will:

1. create a basic CloudFront distribution
2. create multiple origins for a distribution
## Introduction

To enable CloudFront you must specify origin servers, like an Amazon S3 bucket or your own HTTP server, from which CloudFront gets your files which will then be distributed from CloudFront edge locations all over the world.

An origin server stores the original, definitive version of your objects. If you're serving content over HTTP, your origin server is either an Amazon S3 bucket or an HTTP server, such as a web server. Your HTTP server can run on an Amazon Elastic Compute Cloud (Amazon EC2) instance or on a server that you manage; these servers are also known as custom origins.

## Create a CloudFront distribution

1. Open the [CloudFront console](https://console.aws.amazon.com/cloudfront/v4/home) .

Note: If this is the first time you are creating a CloudFront distribution, you may be presented with the Amazon CloudFront Overview page that includes pricing, benefits, and use cases. In such case please click on Create a CloudFront Distribution in the upper right hand corner of the page.

Otherwise, click on the Create Distribution button on the Distributions page.

2. Under Origin Settings, for Origin Domain Name, choose the Amazon S3 bucket that was created by the CloudFormation template used during the prepartion stage. The bucket name will be similar to the following example: **{stack-name}-originbucket-{random-string}.s3.us-east-1.amazonaws.com**. Use `s3Origin` as **Name** of the origin. For the other settings under Origin Settings, accept the default values.
3. For the settings under Default Cache Behavior Settings, accept the default values.
    
4. For Web Application Firewall (WAF) select the "Do not enable security protections" option.
5. For the settings under Distribution Settings, input `index.html` as **Default root object** and accept the default values for rest.
6. At the bottom of the page, choose Create Distribution. This should bring you to the CloudFront Distribution General Settings page similar to the following:
7. After CloudFront creates your distribution, click on the Distributions link in the left menu to go back to the list of **Distributions**. Make sure that the value of the Last modified column for your distribution has changed from Deploying to a specific date time. This typically takes a few minutes.
Record the domain name that CloudFront assigns to your distribution, which appears in the list of distributions. (It also appears on the General tab for a selected distribution.) It looks similar to the following: d111111abcdef8.cloudfront.net.

From now on, we will call this distribution the `CloudFront Distribution` throughout the workshop.

# Create multiple origins
In the previous step, you have seen how to create a CloudFront Distribution that delivers objects from an S3 bucket. Distributions can have more than one origin and can reach to different origins based on the request path.
#### Challenge

Sample website expects to call API with the URI such as _/api/echo_, _/api/login_, etc. Also it attempts to load the video from _/out/<...>_. Change your CloudFront Distribution to accomodate these requirements.

[

#### Step-by-step guide

##### Part 1. Adding new origins

##### API Origin

1. Gather the API Gateway URL from the Output of the CloudFormation template that was created during our preperation phase:
2. Open the `CloudFront Distribution`.
3. Select **Origins** tab.
4. Click **Create origin** button. Create Origin page will be shown.
5. For **Origin domain**, input the domain name of `[apiOriginEndpoint]` from CloudFormation output. Ensure you use only as input. 
```
<a1234abcd>.execute-api.us-east-1.amazonaws.com
```
6. Set **Protocol** to _HTTPS Only_.
7. Set **Name** as _apiOrigin_.
8. Leave others as it is and click **Create Origin**. CloudFront Distribution detail page will be shown.
9. Click **Create origin** button again in the CloudFront Distribution detail.

##### Video Origin


1. Gather the video streaming url from the Output of the CloudFormation template that was created during our preperation phase:
2. 1. Input domain name of `[videoOriginDomain]` from CloudFormation output as **Origin domain**. Again, only Ensure you only use as input.
```
_<abcd1234>.egress.mediapackage-vod.us-east-1.amazonaws.com_ 
```
1. Set **Protocol** as _HTTPS Only_
2. Set **Name** as _videoOrigin_.
3. Leave others as it is and click **Create origin** to return the CloudFront Distribution detail page.

##### Part 2. Route requests to new origins

1. Select **Behaviors** tab.
2. Click **Create behavior** button. Create Behavior page will be shown.
3. Set **Path pattern** as _api/*_.
4. Choose _apiOrigin_ as **Origin and origin group**.
5. Select _GET, HEAD, OPTIONS, PUT, POST, PATCH, DELETE_ as **Allowed HTTP methods**.
6. Select _CachingDisabled_ as **Cache policy**.
7. Select _None_ as **Origin request policy - optional**.
8. Leave others as it is and click **Create behavior** button to go back to CloudFront Distribution detail.
9. Click **Create behavior** button one more time.
10. Set _out/*_ as **Path pattern**.
11. Choose _videoOrigin_ as **Origin and origin group**.
12. Select _CachingOptimized_ as **Cache policy**.
13. Leave others as it is and click **Create behavior** button.
14. Ensure newly created behaviors are above the _Default (*)_ Behavior.
15. Go to **General** tab, and verify whether the **Last modified** is shown as _Deploying_.


#### Testing multiple origins

Once the CloudFront Distribution is deployed, open the test domain (_d1234.cloudfront.net_) again.  
When you reach API menu, you will be able to see some information like below.

Also, when you open Media menu, it will get the play URL after loading the page, and you will be able to play video.