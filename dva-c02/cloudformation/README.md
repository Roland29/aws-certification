# Cloudformation

<details>
 <summary><i>Menu</i></summary>

- [Cloudformation](#cloudformation-1)
</details>

---
## Cloudformation
- Resources
- Parameters
  - !Ref
- Pseudo-partameters
  - AWS::AccountId
- Mappings
  - FindInMap
  - ![cloudformationMapping](../../images/cloudformationMappings.png)
- Outputs
  - export
  - !ImportValue
- Conditions
  - Fn::And
  - Fn::Or
  - Fn::If
  - Fn::Not
  - Fn::Equals
  - ![conditionsStatement](../../images/CF_conditions1.png)
  - ![conditionsApply](../../images/CF_conditions2.png)
- Other functions
  - Fn::Sub
  - Fn::Join
- ChangeSet
  - to see the next modification of the stack before apply
- Stack type
  - Nested stacks
  - Cross stacks
  - StackSet -> share between Multiple AWS account
- Drift
  - Detect manual modification of the stack
- Stack policies
  - if activated, DENY * by default and need ALLOW in policies
