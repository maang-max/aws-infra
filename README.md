#  BUILD AWS INFRASTRUCTURE 
## This repo contains a terraform code to deploy the main infrastructure




Make sure you have the terrafom instaled the AWS credentials configured on your laptop,


- Terraform 
- AWS Cli
- Terramate (optional)

## VPC
- 3 public subnets 1 per AZ
- 3 private subnets 1 per AZ
- 1 NAT Gateway
- 1 Internet Gateway
- Route Tables Associated
## ECS CLUSTER
- with Auto Acaling group capacity provider and AWS CloudWatch Container Insigths
- IAM role
- CloudWatch log groups
- CloudMapb service discovery

Markdown is a lightweight markup language based on the formatting conventions

## Installation

Clone the repo [github](https://github.com/maang-maax/aws-infra/).

Install the dependencies modules and provider

```sh
cd aws-infra
terraform init

```

Review the terrform plan output at the changes

```sh
terraform plan
```
Execute and apply the changes

```sh
terraform apply --auto-approve
```

## Output
You can use this infrastructure, all you need is the cluster_name 

## Cleanup
```sh
terraform destroy
```
## Requirements

Terraform  >= 1.0
aws >= 1.0
## Providers
aws >= 5.0


## License

MIT
