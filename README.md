# Riyaz Ahmed - Cloud & AI SecOps Portfolio

**[LinkedIn Profile](https://www.linkedin.com/in/riyaz-ahmed-572413377)** | **Riyazmalik24680@gmail.com**

### Objective

A recent graduate with Google Cybersecurity and Data Analytics Professional Certificates seeking to apply extensive, hands-on project experience in large-scale log analysis with BigQuery, developing AI-powered detections with Vertex AI, and automating security workflows in Google Cloud.

This portfolio acts as a central hub for my hands-on security projects. Each project is maintained in its own repository.

---

### Core Technical Expertise

* **Cloud & Security Platforms:** Google Cloud Platform (GCP), Chronicle SIEM, Security Command Center, Compute Engine, Cloud Functions, BigQuery, VPC Security, IAM, Identity-Aware Proxy
* **Development & Automation:** Python (Advanced), SQL (Expert), Bash, YAML, JSON, REST APIs
* **AI/ML Technologies:** Vertex AI, TensorFlow, Generative AI APIs, MLOps, Prompt Engineering
* **Security Operations:** SIEM, Threat Hunting, Incident Response, Security Analytics, User Behavior Analytics (UBA), Threat Intelligence
* **Frameworks & Concepts:** NIST CSF, SOC 2, ISO 27001, Zero Trust Architecture

---

## Academic & Security Lab Projects

Here are the projects that demonstrate my skills. Each project is in its own repository, which contains the relevant code and documentation.

### 1. Detection of Shadow AI & Unsanctioned SaaS (Network Log Analysis)

* **Goal:** Used SQL threat-hunting queries in BigQuery to analyze ingested VPC Flow and Cloud DNS logs.
* **Outcome:** Successfully detected network traffic patterns indicative of unsanctioned Generative AI tools (e.g., Grok, Claude), proving the ability to mitigate data exfiltration risks.
* **Key Technologies:** BigQuery, SQL, Cloud Logging (Log Sinks), VPC Flow Logs, Cloud DNS.
* **Code:** **[View Project Repository](https://github.com/Riyaz246/shadow-ai-detection-project)**

### 2. Data-Driven Threat Hunting Pipeline (Detection Engineering)

* **Goal:** Built an end-to-end analytics pipeline by sinking Cloud Storage Data Access audit logs to BigQuery.
* **Outcome:** Developed and operationalized a SQL query to hunt for a simulated data exfiltration breach. This hunt was converted into a real-time Cloud Monitoring alert, automating the incident detection workflow.
* **Key Technologies:** BigQuery, SQL, Cloud Logging (Log Sinks), Cloud Storage, Cloud Monitoring, IAM Audit Logs.
* **Code:** **[View Project Repository](https://github.com/Riyaz246/gcp-data-theft-hunt)**

### 3. Automated Threat Intelligence Firewall (SOAR Pipeline)

* **Goal:** Built a serverless SOAR pipeline to automate network protection.
* **Outcome:** Wrote a Python Cloud Function to fetch a live third-party threat intelligence blocklist. The function automatically updates a GCP "Deny" VPC firewall rule via the Compute Engine API. The pipeline is fully orchestrated with Cloud Scheduler.
* **Key Technologies:** Python, Cloud Functions, Cloud Scheduler, Compute Engine API, VPC Firewall, IAM.
* **Code:** **[View Project Repository](https://github.com/Riyaz246/gcp-automated-firewall)**

### 4. NYC Citi Bike Analysis (Large-Scale UBA)

* **Goal:** Applied SecOps UBA principles to a non-security dataset to prove methodology.
* **Outcome:** Analyzed 50M+ records in BigQuery to perform User Behavior Analytics (UBA), establishing behavioral baselines for distinct user groups. This demonstrates the ability to handle terabyte-scale log volumes and baseline entity groups (e.g., 'Admins' vs. 'Developers') to find insider threats.
* **Key Technologies:** BigQuery, SQL.
* **Code:** **[View Project Repository](https://github.com/Riyaz246/nyc-citibike-analytics-portfolio)**

### 5. Fortified Cloud Web Application (Cloud Hardening & Zero Trust)

* **Goal:** Hardened a vulnerable Compute Engine web server using a secure-by-design, zero-trust approach.
* **Outcome:** Replaced public firewall rules (0.0.0.0/0) with Identity-Aware Proxy (IAP) for SSH. Applied the principle of least privilege to the service account and built Cloud Monitoring alerts to detect failed SSH login attempts.
* **Key Technologies:** GCP, Compute Engine, VPC Firewall, IAM, Cloud Monitoring.
* **Code:** **[View Project Repository](https://github.com/Riyaz246/gcp-security-project)**

### 6. E-commerce Dashboard (Correlated Log Analysis)

* **Goal:** Demonstrated the ability to join and analyze disparate data sources to find anomalies.
* **Outcome:** Correlated and validated data from four disparate tables using SQL `JOINS` to build a unified event timeline. This is the core skill required for joining security logs (e.g., Cloud Audit Logs, VPC Flow Logs, EDR data) to spot genuine threats.
* **Key Technologies:** BigQuery, SQL.
* **Code:** **[View Project Repository](https://github.com/Riyaz246/ecommerce-sales-analytics-portfolio)**

### 7. Hacker News Analysis (Advanced UBA Baselining)

* **Goal:** Used advanced SQL to perform user behavior baselining.
* **Outcome:** Leveraged advanced SQL (CTEs, Window Functions) in BigQuery to analyze and baseline user behavior. This demonstrates the SQL skills required to hunt for anomalous user behavior (e.g., "top 10 hosts with failed logins") in security logs.
* **Key Technologies:** BigQuery, Advanced SQL.
* **Code:** **[View Project Repository](https://github.com/Riyaz246/hacker-news-analytics-portfolio)**

---

### What I'm Building Next

* **AI-Powered Alert Triage:** I am currently developing a new project to enhance my detection pipelines. When a Cloud Monitoring alert fires, it will trigger a Cloud Function that sends the alert data to the **Vertex AI Gemini API**. Using prompt engineering, the AI will act as a Tier 2 Analyst to automatically summarize the threat, map it to the MITRE ATT&CK framework, and suggest remediation steps.
