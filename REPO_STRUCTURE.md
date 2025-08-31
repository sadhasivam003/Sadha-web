# Recommended Repo Structure

- terraform/
  - modules/
    - aws/
    - azure/
    - gcp/
  - envs/
    - dev/
    - test/
    - prod/
- test/
  - terratest/
    - aws_test.go
    - azure_test.go
    - gcp_test.go
- .github/
  - workflows/
    - ci-cd.yml
- go.mod
- README.md

# Key Points
- Place reusable Terraform modules in `terraform/modules`.
- Environment-specific configs in `terraform/envs/{dev,test,prod}`.
- Terratest Go tests in `test/terratest/`.
- CI/CD workflow in `.github/workflows/ci-cd.yml`.
