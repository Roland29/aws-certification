CloudFront
-
- CDN
- S3 origin
- GeoRestriction
- Price location
  - Class ALL
  - Class 200
  - Class 100
- Cache invalidation
- Unicast IP / Anycast IP
- supports HTTP/RTMP protocol based requests

AWS Global Accelerator
-
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