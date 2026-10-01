# Task 01: AWS CLI setup and cost guard

- Installed AWS CLI v2 in WSL2
- Created IAM user `devops-admin` (no root for daily work), root MFA enabled
- Configured the CLI (region ap-south-1) and locked credentials file permissions (chmod 600)
- Verified identity with `aws sts get-caller-identity`
- Created a $10 monthly AWS Budget with an email alert at 80%
