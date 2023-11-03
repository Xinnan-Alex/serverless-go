# Serverless Go with AWS Lambda + API Gateway
- API Gateway
- AWS Lambda
- DynamoDB

This is a simple CRUD API that is deployed to AWS Lambda Function and connected to API Gateway.

Database used is DynamoDB (NOSQL Database)

**IMPORTANT**<br>
Build your Go binary with `GOOS=linux GOARCH=amd64 CGO_ENABLED=0 go build -o build/ cmd/main.go`

GOOS=linux: This is an environment variable that specifies the target operating system for the binary. In this case, it's set to "linux," indicating that the binary will be built to run on a Linux operating system.

GOARCH=amd64: This is another environment variable that specifies the target architecture for the binary. "amd64" represents the 64-bit x86 architecture, commonly used in most modern computers.

CGO_ENABLED=0: This environment variable disables the use of cgo, which is the part of the Go toolchain that allows Go code to call C functions. Setting it to 0 means that cgo is disabled.

Official Documentaiton for deploying GO with AWS Lambda Function
https://docs.aws.amazon.com/lambda/latest/dg/golang-package.html