# GoLang-AWS-Lambda-code-sample

## Description:
This is a production-ready aws lambda template for Go (programming language).

## Why use Go for AWS?
Go is a natively supported language for AWS, and therefore operates faster than languages such as C/C++, because there is basically no "cold start" in the native environment.

## Isn't Go no longer supported?
While it's true that the first version of Go is no longer supported by the AWS SDK (Go v1), the second (and latest) version is still supported, and will likely continue being supported, as important cloud tools - like Terraform (by HashiCorp) - are actually written (at least partially) in Go.

## Usage:
1. Clone and change whatever you need, then zip the app code. 
2. Create a new aws lambda (from either terraform or the AWS console) and upload the code .zip to it

<br>
The usage here can differ depending on what you'd like to do. If it's hosting an API, you can set up an API Gateway to forward requests to a specific lambda. You could also have your go routine listen to an SQS queue, and then take those inputs and write them to DynamoDB tables, etc.
<br>
Remember that Go and AWS create an Event-Driven-Architecture (EDA), where code doesnt run permanently (And shouldn't, for cost reductions). Code is only run in response to an event.
