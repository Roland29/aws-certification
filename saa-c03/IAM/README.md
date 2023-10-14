IAM users
-
- 

IAM Roles
-
- delegate access to users or services that normally don't have access to your organization's AWS resources
- IAM users or AWS services can assume a role to obtain temporary security credentials that can be used to make AWS API calls
- it is possible to access cross-account resources


IAM Advanced
-
- ex: IAM role that you create for the Lambda function is in the same AWS account as the bucket, then you don't need to grant Amazon S3 permissions on both the IAM role and the bucket policy.
- AWS Organisation
  - Consolidated billing across account
  - Shared reserved instances and saving plans
  - Security: Service Control Policies (SCP)
  - Organisation Unit
- IAM Conditions
  - aws:SourceIp
  - aws:RequestedRegion
  - ec2:ResourceTag
  - aws:MultiFactorAuthPresent
  - aws:PrincipalOrgID
- IAM Roles vs Resource Based Policies
  - Using a role as proxy
  - EventBridge - Security
    - Rules:
      - Resource-base policy
      - IAM role
- IAM Permission boundaries
  - for users & roles (not groups)
- IAM Identity Center
  - Replace SSO
  - Fine-grained Permissions and Assignments
    - Multi-Account Permissions
    - Application Assignments
    - Attribute-base Access Control (ABAC)
- AWS Directory Services
  - Managed Microsoft AD
  - AD Connector
    - Just a proxy to on-prem AD
  - Simple AD
- AWS Control Tower
  - Set up and govern a secure and compliant multi-account based on best practices
  - Guardrails
    - Preventive Guardrail - using SCP
    - Detective Guardrail - using AWS Config