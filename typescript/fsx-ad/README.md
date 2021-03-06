# FSx for Windows File Server in AWS Managed Microsoft AD
<!--BEGIN STABILITY BANNER-->
---

![Stability: Stable](https://img.shields.io/badge/stability-Stable-success.svg?style=for-the-badge)

> **This is a stable example. It should successfully build out of the box**
>
> This examples does is built on Construct Libraries marked "Stable" and does not have any infrastructure prerequisites to build.

---
<!--END STABILITY BANNER-->

This example creates an [AWS Managed Microsoft AD](https://aws.amazon.com/directoryservice/active-directory/) and generates an admin password which will be stored in [Secrets Manager](https://aws.amazon.com/secrets-manager/). 

Next, it will provision a multi-az [FSx for Windows File Server](https://aws.amazon.com/fsx/windows/) file system 

## Build

To build this app, you need to be in this example's root folder. Then run the following:

```bash
npm install -g aws-cdk
npm install
npm run build
```

This will install the necessary CDK, then this example's dependencies, and then build your TypeScript files and your CloudFormation template.

## Deploy

Run `cdk deploy`. This will deploy / redeploy your Stack to your AWS Account.

## Synthesize Cloudformation Template

To see the Cloudformation template generated by the CDK, run `cdk synth`, then check the output file in the "cdk.out" directory.