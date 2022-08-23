# How to deploy an Apache web server on AWS EC2 using Terraform

## Description

This is a snippet I collected from the "Terraform Crash Course" by Sanjeev Thiyagarajan

https://www.youtube.com/watch?v=SLB_c_ayRMo

## Reference Material

https://github.com/Sanjeev-Thiyagarajan/Terraform-Crash-Course

## Reference Terraform Commands

https://registry.terraform.io/providers/hashicorp/aws/latest/docs

https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance

terraform init

terraform plan

terraform apply

terraform destroy

https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc

https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet

terraform apply --auto-approve

terraform state list // list all resources

terraform state show aws_eip.one // list details for a resource

terraform -help

terraform destroy -target aws_instance.web-server-instance

terraform apply -target aws_instance.web-server-instance

terraform apply -var "subnet_prefix=10.0.1.0/24"

terraform apply -var-file=terraform.tfvars