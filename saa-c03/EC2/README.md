Launch Instance
-
- It's an instance configuration template that an Auto Scaling group uses to launch EC2 instances.
- Specify:
  - ID of the AMI (Amazon Machine Image)
  - instance type
  - key pair
  - security group
- Can't modify a launch configuration once it is created!

User Data
-
- By default, scripts entered as user data are executed with root user privileges
- By default, user data runs only during the boot cycle when you first launch an instance
- Update your configuration to ensure that your user data scripts and cloud-init directives run every time you restart your instance