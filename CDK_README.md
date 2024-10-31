# CDK Cheatsheet

## Prerequisites
1. node, npm
2. python if you choose verson 3.6 >
3. AWS Cli 
4. AWS CDK Cli

## Install CDK

`npm install -g aws-cdk`

`cdk init app --language python`

Check AWS env for current account
```
aws sts get-caller-identity --query "Account" --output text

aws configure get region
```
### Bootstrap CDK  
`cdk bootstrap aws://123456789012/us-east-1` - one time for environment. from root of your cdk project

`cdk list` - list stacks from project

`cdk synth` - when you have more than one stack, provide name of the stack as parameter or * for all

`cdk deploy` - if you have multiple stack then specify stack name or * for all
