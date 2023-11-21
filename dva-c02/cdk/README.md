# AWS Cloud Development Kit

<details>
 <summary><i>Menu</i></summary>

- [CDK](#cdk)
</details>

---
## CDK
- Define your cloud infrastructure using a familiar language
- Contains high level components called __constructs__
- The code is “compiled” into a CloudFormation template (JSON/YAML)
- ![cdk](../../images/cdk.png)
- cmd
  - ![cdk cmd](../../images/cdkCmd.png)
- Test
  - To import a template
    - Template.fromStack(MyStack) : stack built in CDK
    - Template.fromString(mystring) : stack build outside CDK

