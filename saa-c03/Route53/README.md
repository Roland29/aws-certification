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