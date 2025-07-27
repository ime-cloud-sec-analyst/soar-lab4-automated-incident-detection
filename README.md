# soar-lab4-automated-incident-detection
SOAR Lab 4 – Building an Automated Incident Detection System using Splunk Enterprise and AWS EC2. This lab simulates real-world cyber events (login failures, malware alerts) using Splunk to detect and report them for SOC/Blue Team operations.
soar-lab4-automated-incident-detection/
├── README.md
├── incident_report_summary.png
├── splunk_event_log_search.png
├── splunk_upload_success.png
├── instance_running.png
├── step1_upload_logs/
│   ├── step1-1.png
│   ├── step1-2.png
│   └── ...
├── step2_config_sourcetype/
│   ├── step2-1.png
│   └── ...
├── step3_create_report/
│   └── ...
├── step4_export_findings/
│   └── ...
├── ec2_instance_launch/
│   └── ...
└── notes.md

# SOAR Lab 4: Automated Incident Detection with Splunk and AWS EC2

This lab demonstrates how to simulate and detect real-world cyber incidents using Splunk Enterprise on an AWS EC2 instance. The environment mimics SOC (Security Operations Center) activities by ingesting logs, identifying suspicious behaviors, and generating incident reports in response to malware detection and login events.

---

## 🎯 Objective

- Upload security logs into Splunk.
- Identify and analyze incident patterns (malware, failed login, etc.).
- Generate summary reports using Splunk Search Processing Language (SPL).
- Simulate real-life SOC use cases using automation tools in AWS.
- Visualize incidents for response and documentation.

---

## 📌 Significance

This lab is essential for understanding:
- How modern SIEM platforms like Splunk work.
- How SOC/Blue Team teams identify threats in real time.
- Hands-on experience with detecting and analyzing attack vectors.
- Bridging the gap between cloud infrastructure and cybersecurity analytics.

---

## 🧰 Tools & Services Used

- **Splunk Enterprise 9.4.3** (on EC2)
- **AWS EC2** (t2.micro instance - Ubuntu)
- **CloudWatch** (for basic metrics)
- **example_logs.txt** (malicious log simulation)

---

## 📝 Summary of Tasks

| Step | Description |
|------|-------------|
| ✅ 1 | Launch EC2 instance and install Splunk Enterprise |
| ✅ 2 | Ingest simulated logs (example_logs.txt) |
| ✅ 3 | Set source type and indexing configurations |
| ✅ 4 | Use SPL search to identify security events |
| ✅ 5 | Generate reports: login failures, malware alerts |
| ✅ 6 | Summarize and export incident count reports |

---

## 🔍 Key Findings

| Time (UTC)        | Event |
|-------------------|-------|
| 12:23:45          | Failed login from 192.168.1.10 to `admin` |
| 12:24:10          | Successful login from 10.0.0.5 to `analyst` |
| 12:25:35          | Malware detected on host WIN-32ABC |

✅ These events were successfully detected and indexed in Splunk.
✅ A count report was generated to track frequency.

---

## 📚 Lessons Learned

- Proper log formatting (timestamp + message) is crucial for Splunk parsing.
- Custom source types help organize and isolate event types.
- Splunk SPL (Search Processing Language) is powerful for real-time threat detection.
- AWS EC2 and CloudWatch provide foundational infrastructure for detection labs.

---

## ⚠️ Limitations

- The logs are synthetic and not based on real-world attack traffic.
- Malware detection is purely simulated — no antivirus or sandbox used.
- No automation was built for alerting or response (e.g., SOAR playbooks).
- CloudWatch usage was minimal — limited to EC2 metrics only.

---

## 🚀 Real-World Implementation Use Case

**Scenario:**  
A Security Operations Center (SOC) receives alert logs from multiple endpoints. Using Splunk, the SOC team:

- Automatically ingests the logs into indexed sources.
- Detects brute-force attempts or malware infections.
- Generates daily reports and raises alerts to incident response teams.

This lab reflects that workflow, helping cloud security analysts build detection logic in the cloud.

---

## 🏁 Take-Home Summary

- You can detect attacks **without expensive tools** using just EC2 + Splunk.
- Hands-on log parsing helps build real SOC analyst skills.
- Every AWS Cloud Security Analyst should practice incident detection.
- Mastering SPL, understanding log types, and setting up alerts are essential skills.

---

## 📷 Screenshots & Evidence

A total of **34 screenshots** are included to demonstrate:

- EC2 instance deployment  
- Splunk setup and log upload  
- Event detection in SPL search  
- Report generation  
- CloudWatch monitoring  

All screenshots are organized by step folders in this repository.

---

## 🗂 Folder Structure


soar-lab4-automated-incident-detection/
├── README.md
├── incident_report_summary.png
├── instance_running.png
├── step1_upload_logs/
├── step2_config_sourcetype/
├── step3_event_search/
├── step4_summary_reports/
├── step5_cloudwatch_metrics/
└── notes.md

✅ Status: Lab Completed Successfully
Please ⭐ the repo if this helps your learning!
Feel free to fork and adapt it for your own use cases.

✍️ Author
Dr. Ime Ben
AWS Cloud Security Analyst
GitHub: ime-cloud-sec-analyst
LinkedIn Profile: www.linkedin.com/in/ime-ben-8aa008362

