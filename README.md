# Riyaz Ahmed - Cloud & AI SecOps Portfolio

**[LinkedIn Profile](https://www.linkedin.com/in/riyaz-ahmed-101)** | **Riyazmalik24680@gmail.com**

### Objective

[span_0](start_span)A recent graduate with Google Cybersecurity and Data Analytics Professional Certificates[span_0](end_span) [span_1](start_span)[span_2](start_span)seeking to apply extensive, hands-on project experience in large-scale log analysis with BigQuery[span_1](end_span)[span_2](end_span)[span_3](start_span), developing AI-powered detections with Vertex AI[span_3](end_span)[span_4](start_span)[span_5](start_span), and automating security workflows in Google Cloud[span_4](end_span)[span_5](end_span).

This portfolio contains the code and documentation for my hands-on security projects.

---

### Core Technical Expertise

* **[span_6](start_span)Cloud & Security Platforms:** Google Cloud Platform (GCP), Chronicle SIEM, Security Command Center, Compute Engine, Cloud Functions, BigQuery, VPC Security, IAM, Identity-Aware Proxy[span_6](end_span)
* **[span_7](start_span)Development & Automation:** Python (Advanced), SQL (Expert), Bash, YAML, JSON, REST APIs[span_7](end_span)
* **[span_8](start_span)AI/ML Technologies:** Vertex AI, TensorFlow, Generative AI APIs, MLOps, Prompt Engineering[span_8](end_span)
* **[span_9](start_span)Security Operations:** SIEM, Threat Hunting, Incident Response, Security Analytics, User Behavior Analytics (UBA), Threat Intelligence[span_9](end_span)
* **[span_10](start_span)Frameworks & Concepts:** NIST CSF, SOC 2, ISO 27001, Zero Trust Architecture[span_10](end_span)

---

## Academic & Security Lab Projects

Here are the projects that demonstrate my skills. Each project folder in this repository contains the relevant `README.md` and code (e.g., `.sql` queries, `.py` scripts).

### 1. Detection of Shadow AI & Unsanctioned SaaS (Network Log Analysis)

* **[span_11](start_span)Goal:** Used SQL threat-hunting queries in BigQuery to analyze ingested VPC Flow and Cloud DNS logs[span_11](end_span).
* **[span_12](start_span)Outcome:** Successfully detected network traffic patterns indicative of unsanctioned Generative AI tools (e.g., Grok, Claude), proving the ability to mitigate data exfiltration risks[span_12](end_span).
* **[span_13](start_span)Key Technologies:** BigQuery, SQL, Cloud Logging (Log Sinks), VPC Flow Logs, Cloud DNS[span_13](end_span).
* **Code:** `[See the SQL queries here](./shadow-ai-detection/)`

### 2. Data-Driven Threat Hunting Pipeline (Detection Engineering)

* **[span_14](start_span)Goal:** Built an end-to-end analytics pipeline by sinking Cloud Storage Data Access audit logs to BigQuery[span_14](end_span).
* **[span_15](start_span)Outcome:** Developed and operationalized a SQL query to hunt for a simulated data exfiltration breach[span_15](end_span). [span_16](start_span)This hunt was converted into a real-time Cloud Monitoring alert, automating the incident detection workflow[span_16](end_span).
* **[span_17](start_span)Key Technologies:** BigQuery, SQL, Cloud Logging (Log Sinks), Cloud Storage, Cloud Monitoring, IAM Audit Logs[span_17](end_span).
* **Code:** `[See the SQL hunt query here](./data-exfil-hunt/)`

### 3. Automated Threat Intelligence Firewall (SOAR Pipeline)

* **Goal:** Built a serverless SOAR pipeline to automate network protection.
* **[span_18](start_span)Outcome:** Wrote a Python Cloud Function to fetch a live third-party threat intelligence blocklist[span_18](end_span). [span_19](start_span)The function automatically updates a GCP "Deny" VPC firewall rule via the Compute Engine API[span_19](end_span). [span_20](start_span)The pipeline is fully orchestrated with Cloud Scheduler[span_20](end_span).
* **[span_21](start_span)Key Technologies:** Python, Cloud Functions, Cloud Scheduler, Compute Engine API, VPC Firewall, IAM[span_21](end_span).
* **Code:** `[See the Python code here](./soar-pipeline/)`

### 4. NYC Citi Bike Analysis (Large-Scale UBA)

* **Goal:** Applied SecOps UBA principles to a non-security dataset to prove methodology.
* **[span_22](start_span)Outcome:** Analyzed 50M+ records in BigQuery to perform User Behavior Analytics (UBA), establishing behavioral baselines for distinct user groups[span_22](end_span). [span_23](start_span)This demonstrates the ability to handle terabyte-scale log volumes and baseline entity groups (e.g., 'Admins' vs. 'Developers') to find insider threats[span_23](end_span).
* **[span_24](start_span)Key Technologies:** BigQuery, SQL[span_24](end_span).
* **Code:** `[See the UBA queries here](./uba-citibike/)`

### 5. Fortified Cloud Web Application (Cloud Hardening & Zero Trust)

* **[span_25](start_span)Goal:** Hardened a vulnerable Compute Engine web server using a secure-by-design, zero-trust approach[span_25](end_span).
* **[span_26](start_span)Outcome:** Replaced public firewall rules (0.0.0.0/0) with Identity-Aware Proxy (IAP) for SSH[span_26](end_span). [span_27](start_span)Applied the principle of least privilege to the service account and built Cloud Monitoring alerts to detect failed SSH login attempts[span_27](end_span).
* **[span_28](start_span)Key Technologies:** GCP, Compute Engine, VPC Firewall, IAM, Cloud Monitoring[span_28](end_span).
* **Code:** `[See hardening config/alerts here](./cloud-hardening-lab/)`

### 6. E-commerce Dashboard (Correlated Log Analysis)

* **Goal:** Demonstrated the ability to join and analyze disparate data sources to find anomalies.
* **[span_29](start_span)Outcome:** Correlated and validated data from four disparate tables using SQL `JOINS` to build a unified event timeline[span_29](end_span). [span_30](start_span)This is the core skill required for joining security logs (e.g., Cloud Audit Logs, VPC Flow Logs, EDR data) to spot genuine threats[span_30](end_span).
* **[span_31](start_span)Key Technologies:** BigQuery, SQL[span_31](end_span).
* **Code:** `[See the correlation queries here](./ecommerce-analysis/)`

### 7. Hacker News Analysis (Advanced UBA Baselining)

* **Goal:** Used advanced SQL to perform user behavior baselining.
* **[span_32](start_span)Outcome:** Leveraged advanced SQL (CTEs, Window Functions) in BigQuery to analyze and baseline user behavior[span_32](end_span). [span_33](start_span)This demonstrates the SQL skills required to hunt for anomalous user behavior (e.g., "top 10 hosts with failed logins") in security logs[span_33](end_span).
* **[span_34](start_span)Key Technologies:** BigQuery, Advanced SQL[span_34](end_span).
* **Code:** `[See the Advanced SQL queries here](./uba-hackernews/)`

---

### What I'm Building Next

* **AI-Powered Alert Triage:** I am currently enhancing the "Data-Driven Threat Hunting Pipeline" project. When a Cloud Monitoring alert fires, it will trigger a Cloud Function that sends the alert data to the **Vertex AI Gemini API**. Using prompt engineering, the AI will act as a Tier 2 Analyst to automatically summarize the threat, map it to the MITRE ATT&CK framework, and suggest remediation steps.
