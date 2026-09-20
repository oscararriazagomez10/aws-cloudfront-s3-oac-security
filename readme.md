# 🔒 Secure Global Static Web Hosting with AWS CloudFront & S3 (OAC)

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)
![CloudFront](https://img.shields.io/badge/CloudFront-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Security](https://img.shields.io/badge/Security-Least_Privilege-red?style=for-the-badge)

> **Elevator Pitch:** A high-security, low-latency static website hosting architecture. The origin storage (**Amazon S3**) remains completely isolated from the public network (`Block ALL Public Access`), routing incoming read traffic exclusively through **Amazon CloudFront** via dynamic authentication with **Origin Access Control (OAC)**.

---

##  Why This Architecture?

In corporate production environments, publicly exposed Amazon S3 buckets represent one of the primary security vulnerabilities leading to data leaks. This architecture addresses two fundamental business problems:

1. **Security & Zero Public Exposure:** Eliminates direct public S3 endpoints, protecting static assets against unauthorized access or scanning attacks.
2. **Global Performance & Availability:** Distributes content across AWS's global network of Edge Locations, significantly reducing latency for end users while minimizing origin request load.

---

## 🏗️ Architecture Diagram

![AWS Architecture Diagram](docs/Architecture
