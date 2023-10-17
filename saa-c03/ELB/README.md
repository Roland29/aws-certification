# Load Balancer

<details>
 <summary><i>Menu</i></summary>

- [ALB](#application-load-balancer-alb)
- [NLB](#network-load-balancer-nlb)
- [GLB](#gateway-load-balancer-glb)
- [ELB](#elastic-load-balancer-elb)
- [ASG](#auto-scaling-group-asg)
</details>

---
## Application Load Balancer (ALB)
- security group
![ALB security group](../../images/ALB_SG.jpg)

---
## Network Load Balancer (NLB)

---
## Gateway Load Balancer (GLB)
- GENEVE protocol 6081
![GLB](../../images/glb.png)

---
## Elastic Load Balancer (ELB)
- sticky Session
  - Application-based Cookies
  - Duration-based Cookies
- Cross zone
    - ALB default
    - NLB (not free)
![cross-zone](../../images/crossZone.png)
- SSL
- Connection Draining

---
## Auto Scaling group (ASG)
- [Launch template](../EC2/README.md#launch-template) 
- Dynamic scaling policies
  - Target tracking scaling
    - based on a Amazon CloudWatch metric
    - and a target value
  - Step scaling
    - base on a set of scaling adjustments that vary based on the size of the alarm breach
  - simple 
    - based on a single scaling adjustment, with a cool down period between each scaling activity
  - scheduled Action
    - scaling action at a certain designated hour
- Predictive Scaling
  - predictive scaling
- Standby mode to update some software
- ReplaceUnhealthy (can be suspended)