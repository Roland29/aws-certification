# Routes 53

<details>
 <summary><i>Menu</i></summary>

- [Types](#types)
- [Policies](#policies)
- [HealthCheck](#healthcheck)
- [TTL](#ttl)
</details>

---
## Types
- A -> IPV4
- AAAA -> IPV6
- CNAME -> redirection but not domain
- Alias -> AWS resources
- NS -> server name

---
## Policies
- Simple
- Weight
- Multi-Value
- Latency
- Fail-over
  - active-passive
    - secondary resource to be on standby in case all the primary resources become unavailable
- Geolocation
- GeoProximity
- IP base routing

---
## HealthCheck
- For VPC -> healthcheck cloudwatch alarm
- Calculate healthCheck -> base on other healthCheck

---
## TTL
- Time to live

---
## Hosted zones
- Public Hosted zones
  - contains records that specify how to route traffic on the Internet (public domain names)
- Private Hosted zones
  - contain records that specify how you route traffic within one or more VPCs (private domain names)
  - DNS hostnames and DNS resolution are required settings for private hosted zones
![public vs private hosted zones](../../images/publicVsPrivate%20HostedZones.png)