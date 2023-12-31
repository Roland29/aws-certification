# AWS CICD

<details>
 <summary><i>Menu</i></summary>

- [CodeCommit](#codecommit)
- [CodePipeline](#codepipeline)
- [CodeBuild](#codebuild)
- [CodeDeploy](#codedeploy)
- [CodeStar](#codestar)
- [CodeGuru](#codeguru)
</details>

---
## CodeCommit
- repo like GitHub but with minimal UI
- Base on Git
- access through ssh or https
  - repositories is encrypted in transit and at rest automatically

---
## CodePipeline
- jenkins

---
## CodeBuild
- buildspec.yml at root of code repo
- Bundle the dependencies in the source code during the build stage
- CodeBuild scales automatically, the organization does not have to do anything for scaling or for parallel builds

---
## CodeDeploy
- appspec.yml
  - AppStop
  - DownloadBundle
  - BeforeInstall
  - Install
  - AfterInstall
  - StartApp
  - validateService
- predefined deployment configurations for EC2/on-premises instances
  - OneAtATime
  - HalfAtATime
  - AllAtOnce
- Deployment with ASG
  - blue-green deployment
  - In-place

---
## CodeStar
- Manage all codePipeline, codeCommit, codeBuild at high level

---
## CodeGuru
- for Java & Python
- CodeGuru Reviewer
- CodeGuru Profiler 