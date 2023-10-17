# CloudFront

<details>
 <summary><i>Menu</i></summary>

- [CloudFront](#cloudfront-1)
- [AWS Global Accelerator](#aws-global-accelerator)
</details>

---
## CloudFront
- CDN
- S3 origin
- DDos protection
- Origin Access Control (OAC)
- GeoRestriction
- Price location
  - Class ALL
  - Class 200
  - Class 100
- Cache invalidation
- Uni cast IP / Any cast IP
- supports HTTP/RTMP protocol based requests
- Region edge cache:
  - __NOT FOR__: Dynamic content, as determined at request time (cache-behavior configured to forward all headers)
  - __NOT FOR__: Proxy methods PUT/POST/PATCH/OPTIONS/DELETE go directly to the origin

---
## AWS Global Accelerator
- Improve the availability and performance of the applications
  - Static IP addresses
    - fixed entry point to your applications
- Routes user traffic to the optimal endpoint based on performance
- Good fit for non-HTTP
  - gaming (UDP), IoT (MQTT), or Voice over IP
- endpoint weights to determine the proportion of traffic
- outputs:
  - ALB
  - NLB
  - EC2