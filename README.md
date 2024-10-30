# GitOps with Terraform 2024 Starter Code

## Cloudformation

The code in the ./cloudformation directory is optional. It is to configure the OIDC role used to authenticate your GitHub Actions workflows to AWS. 

## Terraform

The code in the ./terraform directory is the starter code for the course. This code isn't perfect, and that's intentional! You may need to make modifications to ensure it is reliable and resilient. 


## GH Actions  Template
https://github.com/actions/starter-workflows/blob/main/deployments/terraform.yml

# Command Hacks

When running teraform fmt...  for e.g. (global usage with ll commands)
```bash
terraform -chdir="./terraform" fmt
```

If `terraform fmt --check` finds linting issues, it will fail in the gha pipeline

https://github.com/terraform-linters/  #mtc

https://github.com/marketplace/actions/tflint-github-action

https://github.com/gruntwork-io/terratest

https://spacelift.io/blog/terraform-precondition-postcondition

