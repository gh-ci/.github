# GH CI

GH CI organization profile and management.

## Features

Organization managed using [GitHub - Xebis: GitHub Organization as Code](https://github.com/xebis/github-organization-as-code) with configuration [`org.yaml`](org.yaml) with these alterations for local use:

- Clone [GitHub - Xebis: GitHub Organization as Code](https://github.com/xebis/github-organization-as-code) on the same level as this repo
- `github-organization-as-code/terraform/config.tf`:
  - Backend S3 configuration: `bucket = "<your bucket>"`
- `TF_VAR_path="../../.github/org.yaml"`
- Terraform command: `terraform -chdir=../github-organization-as-code/terraform init/plan/apply/...`
