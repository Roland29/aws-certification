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

---
## CodePipeline
- jenkins

---
## CodeBuild
- buikdspec.yml at root of code repo

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

---
## CodeStar
- Manage all codePipeline, codeCommit, codeBuild at high level

---
## CodeGuru
- for Java & Python
- CodeGuru Reviewer
- CodeGuru Profiler 