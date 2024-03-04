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
3. Create an API Gateway that will call this lambda function, and test
