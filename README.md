<!-- Profile README for github.com/ThomasTafa29 · Last updated: November 2026 -->

<h1 align="center">Thomas Tafa</h1>

<p align="center">
  <strong>IT Professional &nbsp;|&nbsp; AWS &amp; Azure &nbsp;|&nbsp; Systems Administration &nbsp;|&nbsp; Healthcare IT &amp; HIPAA</strong>
  <br>
  Brooklyn, NY &nbsp;·&nbsp; Open to remote or NYC-hybrid roles
</p>

<p align="center">
  <!-- TODO: replace YOUR-LINKEDIN-HANDLE with the end of your LinkedIn profile URL (appears twice in this file) -->
  <a href="https://www.linkedin.com/in/thomas-tafa/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Thomas%20Tafa-0A66C2?style=flat-square"></a>
  <a href="mailto:thomastafa21@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-thomastafa21%40gmail.com-555555?style=flat-square"></a>
  <img alt="AWS Certified Cloud Practitioner" src="https://img.shields.io/badge/AWS-Certified%20Cloud%20Practitioner-FF9900?style=flat-square">
</p>

---

## About me

I'm an IT professional with close to four years of experience supporting users, systems, and infrastructure in healthcare and higher education. I'm moving into cloud and systems administration, and this GitHub is where I document that work: real builds, real troubleshooting, and a recorded walkthrough for each project.

- **Currently:** IT Service Technician at LaGuardia Community College (CUNY)
- **Previously:** Clinical Systems Support Analyst at Maimonides Medical Center (~2.5 years), supporting EHR and clinical systems in a HIPAA-regulated hospital, including a live Emergency Department buildout
- **Cloud training:** AWS re/Start (Per Scholas) and a 7-month AWS Cloud Engineering Fellowship (Silver Lining Program)

Working in a hospital shaped how I approach infrastructure. Downtime affects patient care, and one access mistake can expose protected health information. I carry that into everything I build: least-privilege access, audit logging, documented changes, and synthetic data only.

---

## Portfolio

### Security & Infrastructure Lab Series

Five connected labs, each building on the last. The domain controller from Lab 1 becomes the log source for Splunk in Lab 3 and the scan target for Nessus in Lab 5. Because I come from healthcare, I map each lab to the HIPAA Security Rule safeguard it exercises.

| Lab | What it covers | HIPAA Security Rule | Status |
|:---:|---|---|:---:|
| **1** | [**Active Directory Domain Lab**](https://github.com/ThomasTafa29/active-directory-domain-lab)<br>Windows Server 2025 domain controller on Azure: OUs, users and security groups, Group Policy, a fine-grained password policy, and account lockout, scripted in PowerShell and verified end to end | §164.312(a)<br>Access Control | ✅ Published<br>+ video |
| **2** | [**Wireshark Network Analysis**](https://github.com/ThomasTafa29/wireshark-network-analysis)<br>DNS resolution, the TCP three-way handshake, and stream reassembly, plus a demonstration of credentials exposed over plain HTTP against a local test server I built | §164.312(e)<br>Transmission Security | ✅ Published |
| **3** | **Splunk SIEM & Log Analysis**<br>Windows Security logs forwarded from the Lab 1 domain controller into Splunk on Ubuntu, with SPL detections for logons, failed logons, and account lockouts, a security dashboard, and a scheduled alert | §164.312(b)<br>Audit Controls | 🔨 In progress |
| **4** | **ServiceNow ITSM**<br>Incident and change management workflows on a ServiceNow developer instance, from intake and prioritization through change approval | §164.308(a)(6)<br>Security Incident Procedures | 🗓️ Up next |
| **5** | **Nessus Vulnerability Scanning**<br>Credentialed scans of the lab environment: prioritizing findings, remediating, and rescanning to confirm the fix | §164.308(a)(1)(ii)(A)<br>Risk Analysis | 🗓️ Planned |
| **★** | **Capstone: Cloud Alert to Incident**<br>CloudWatch alarm → SNS → Lambda → automatic ServiceNow incident, connecting cloud monitoring to the ITSM workflow from Lab 4 | §164.308(a)(6)<br>Security Incident Procedures | 🗓️ Planned |

<sub>Lab environments built with synthetic data. The mappings show which safeguard each lab exercises; they are not compliance claims.</sub>

### AWS Cloud Projects

Originally built during my AWS fellowship in sandbox accounts that have since closed. I'm rebuilding each one in my own AWS account as a public repo with infrastructure as code, an architecture diagram, and a teardown plan.

| Project | What it shows | Status |
|---|---|:---:|
| **Serverless resume site with a HIPAA-aligned security layer** | Private S3 behind CloudFront (Origin Access Control), a Lambda + DynamoDB visitor counter, KMS customer-managed keys, CloudTrail, and AWS Config. Deployed by GitHub Actions with OIDC, so no long-lived access keys | 🔨 Rebuilding |
| **Containerized CI/CD pipeline** | A Python Flask app built and deployed to ECS Fargate through CodePipeline, CodeBuild, and ECR, with all infrastructure in Terraform | 🔨 Rebuilding |
| **Three-tier VPC architecture** | Web, app, and database tiers across two Availability Zones: Application Load Balancer, EC2 Auto Scaling, and RDS Multi-AZ, defined in CloudFormation. Includes a cost review with Cost Explorer, Trusted Advisor, and S3 lifecycle policies | 🔨 Rebuilding |

---

## Technical skills

| Area | Tools and technologies |
|---|---|
| **AWS** | EC2, VPC, S3, IAM, RDS, Lambda, CloudFront, CloudWatch, SNS, Auto Scaling, Cost Explorer, Trusted Advisor |
| **Azure** | Virtual Machines, Virtual Networks, Network Security Groups, resource groups, cost management |
| **Infrastructure as Code & CI/CD** | Terraform, AWS CloudFormation, GitHub Actions, Docker, Git |
| **Scripting** | PowerShell, Python, Bash, SQL |
| **Identity & Systems** | Active Directory Domain Services, DNS, Group Policy, Fine-Grained Password Policies, Windows Server 2025, Ubuntu Linux |
| **Security & Monitoring** | Splunk (SPL, Universal Forwarder), Wireshark, Windows Event Logs |
| **IT Support & Healthcare IT** | End-user and desktop support, clinical and EHR systems support, troubleshooting and escalation, HIPAA-regulated environments |

---

## Certifications & training

| | Credential | Issuer |
|:---:|---|---|
| ✅ | AWS Certified Cloud Practitioner | Amazon Web Services |
| ⏳ | AWS Certified Solutions Architect – Associate (SAA-C03), exam scheduled November 2026 | Amazon Web Services |
| ✅ | IBM AI Practitioner | IBM |
| 🗓️ | Microsoft Azure Administrator (AZ-104), planned | Microsoft |
| 🎓 | AWS Cloud Engineering Fellowship (7 months) | Silver Lining Program |
| 🎓 | AWS re/Start | Per Scholas |

<!-- After you pass SAA-C03: change ⏳ to ✅, delete ", exam scheduled November 2026", and add a matching badge at the top. -->

---

## How I document my work

Every repo on this profile is built to the same standard:

- An architecture diagram and the reasoning behind each design decision
- Commented scripts and infrastructure as code
- Screenshots with IPs, hostnames, and credentials redacted
- A troubleshooting log of what broke and how I fixed it
- A recorded video walkthrough explaining the build
- Synthetic data only: no credentials, keys, or real patient data, ever

---

## Let's connect

I'm open to Cloud Support, Cloud Operations, and Systems Administration roles, remote or hybrid in the NYC area. Healthcare and health-tech teams are a natural fit for my background. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/YOUR-LINKEDIN-HANDLE) or [email](mailto:thomastafa21@gmail.com).
