# Mission 02 — Field Guide Update

## Useful Command/Tool

`curl.exe http://metadata.services.cityinthe.cloud:1338/latest/meta-data/instance-type`

**Use:** Retrieves EC2 instance metadata such as the instance type.

## Vulnerability-Prioritization Concept

CVSS does not automatically determine priority. Consider exposure, asset criticality, active exploitation, and compensating controls.

## Useful Port/Service or Reconnaissance Discovery

AWS EC2 Instance Metadata Service (IMDS) — provides instance information such as availability zone, IAM role, instance type, and AMI information.

## Troubleshooting Lesson

**Problem:** I initially had trouble determining which metadata paths to query.

**Cause:** Different information is stored under different metadata endpoints.

**Fix:** Start with the metadata path and identify the specific category of information needed.

**Remember:** Check the metadata path carefully when the first query does not give the expected information.

## Worth Remembering

When performing reconnaissance, identify what information you already have, what information is missing, and which tool or endpoint can provide it.
