@technovangelist

# What is Serverless
Yes, it is Serverless as far as you are concerned
Don't pay for idle
- unlike on EC2 or others. 
Scale with ease
FaaS - Function as a Service

# Supported Languages
AWS
- NodeJS
- Python
- Java
- Go 
- C#

Azure
- NodeJS
- C#
- F#

Google Cloud
- NodeJS

# Supported Triggers
AWS
- S3
- DynamoDB
- Kinesis
- SNS
- SES
- Cognito
- Cloudwatch Logs
- Cloudwatch Events
- CodeCommit
- Config
- Alexa
- Lex
- API Gateway
- 



# Your first Lambda
Serverless Application Repository - ready to go apps built by others
Blueprints - Kinda like sample code
Author from scratch - build your own
- Pick a good name, so you know what the hell is what later
- Pick a runtime
Role
- Usually just starts with a template for ease

# Your first Azure Function
Azure Portal -> Create a resource
Function App
- inside app add more functions
- all functions kind of stay in this bundle
Container
- you can choose your own container
functionlibrary.azurewebsites.net

# Your first Google Cloud Function


...serverless functions should respect the single responsibility principle...
- single responsibility principle = every function should do 1 thing (1 thing varies depending on granularity)

AWS - Step Functions
Azure - Logic Apps & Microsoft Flow
Google - ?

serverlesscalc.com
- calculates cost for serverless use cases

Process on AWS
1. Create S3 Bucket
Push web page content to S3
Set permissions (cors, public read)
Create DynamoDB
Create Lambda (and write the function)
Set Permissions
More stuff

Process on Azure
Create Azure Function App
Create page serving function (copy/paste boilerplate)
Upload content to App
Add a Proxy in the App (friendlier URL)
Add a Table 
More Stuff

# Serverless Framework to the rescue?
- great on AWS due to plugins
- everything else not so much

You >COULD< mix and match
http://bit.ly/khmix
- Kelsey Hightower
- Not so FaaS

Datadog
Splunk


Look for awesome-<anything> and you'll find some awesome stuff