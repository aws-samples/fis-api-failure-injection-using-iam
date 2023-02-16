# Validate resilience at API boundaries with AWS Fault Injection Simulator and IAM policies

This repo contains AWS CloudFormation templates supporting a blog post (link TBD) about extending AWS Fault Injection Service fault injections by modifying IAM policies. 

This code is released under [MIT-0 license](LICENSE.md). 

Please see the blog post for how to use these templates.

## Deployment

Deploy the templates with 

```bash
aws cloudformation deploy \
  --stack-name test-fis-api-faults \
  --template-file template.yaml \
  --capabilities CAPABILITY_NAMED_IAM
```

and

```bash
aws cloudformation deploy \
  --stack-name test-fis-api-faults \
  --template-file template2.yaml 
  --capabilities CAPABILITY_NAMED_IAM
```

