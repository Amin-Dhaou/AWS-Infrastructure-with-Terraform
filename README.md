# 🚀 AWS Infrastructure with Terraform (VPC + ALB + AutoScaling + IAM + WAF)

This project automates the deployment of a complete AWS infrastructure using Terraform. It includes:

- A VPC with subnet and internet access  
- EC2 instances managed by Auto Scaling  
- An Application Load Balancer (ALB)  
- Web Application Firewall (WAF) integrated with the ALB  
- IAM users, groups, and policies  

## ⚙️ Prerequisites

- [Terraform](https://developer.hashicorp.com/terraform/downloads) installed  
- An AWS account with programmatic access  
- Optional: AWS CLI installed and configured

## 📁 Structure

This is a single-file Terraform configuration (`main.tf`) with all resources included. You can extend it with `modules/` and `environments/` folders for production use.

## 🧪 Terraform Workflow

# Cloner le projet depuis GitHub
git clone https://github.com/your-username/aws-terraform-infra.git && cd aws-terraform-infra

# (Optionnel) Exporter les clés AWS si non configurées via aws-cli
export AWS_ACCESS_KEY_ID="votre_access_key"
export AWS_SECRET_ACCESS_KEY="votre_secret_key"

# Initialiser Terraform
terraform init

# Afficher les changements prévus
terraform plan

# Appliquer la configuration (taper 'yes' quand demandé)
terraform apply

# Afficher la sortie avec le DNS du Load Balancer
terraform output

# Pour tout détruire (taper 'yes' quand demandé)
# terraform destroy

