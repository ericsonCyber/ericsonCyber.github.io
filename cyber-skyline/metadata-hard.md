# Cyber Skyline – Metadata (Hard)

## Challenge

**Category:** Scanning & Reconnaissance  
**Challenge:** Metadata

This challenge involved enumerating an AWS EC2 Instance Metadata Service endpoint.

---

## Questions & Answers

### 1. What availability zone is this instance hosted in?

**Answer:** `us-west-2a`

**Command used:**
```powershell
curl.exe http://metadata.services.cityinthe.cloud:1338/latest/meta-data/placement/availability-zone
### 2. What IAM role is attached to this instance?

**Answer:** `liber8-role`

**Command used:**

```powershell
curl.exe http://metadata.services.cityinthe.cloud:1338/latest/meta-data/iam/security-credentials
---
### Next question
### 3. What is the instance type?

**Answer:** `c6g.16xlarge`

**Command used:**

```powershell
curl.exe http://metadata.services.cityinthe.cloud:1338/latest/meta-data/instance-type
---
### Next question
### 4. What is the operating system name and version number?

**Answer:** `Ubuntu 16.04`

**Command used:**

```powershell
curl.exe http://metadata.services.cityinthe.cloud:1338/latest/meta-data/ami-id
---
### Next question
### 5. What was the flag?

**Answer:** `SKY-AWSM-1570`

**Command used:**

```powershell
curl.exe http://metadata.services.cityinthe.cloud:1338/latest/meta-data/network/interfaces/macs/0e:49:61:0f:c3:11/vpc-ipv4-cidr-blocks

That's **three backticks**. The backtick key is usually **directly below Esc**, to the left of the `1` key.

So the bottom should look like:
