# Incident Handling 101: Tactical Playbook

A technical reference platform documenting the **NIST SP 800-61** lifecycle. I built this to bridge the gap between cybersecurity theory and the practical response scripts used during breach containment.

**[Live Site](https://dhi0grk4hu2h4.cloudfront.net/)**

---

### 🛠️ Technical Features
* **IR Lifecycle Documentation:** Detailed walk-throughs for Preparation, Detection, Containment, and Recovery.
* **Practical Tooling Examples:** The playbook includes implementation logic for:
    * **YARA Rules** for pattern-based RAT detection.
    * **PowerShell** scripts for rapid multi-endpoint IOC scanning (hashes and processes).
    * **Memory Forensics** logic (Volatility) to identify stagers and fileless malware.
* **Case Analysis:** Deep dive into the **Colonial Pipeline** ransomware attack and the **Cyber Kill Chain** framework.

### ☁️ Cloud & Security
I hosted this platform on AWS to gain experience with secure, production-grade cloud deployments:
* **Architecture:** Static hosting via **S3** and **CloudFront** (for global CDN and SSL/TLS).
* **Infrastructure as Code (IaC):** I included a **CloudFormation** template to manage the S3 Bucket Policy. 
* **Security Principle:** The policy enforces the **Principle of Least Privilege**, restricting public access strictly to the `/public/*` assets folder to prevent "leaky bucket" misconfigurations.

### 📂 Repository Structure
* `index.html`: Core playbook content and NIST documentation.
* `css/` & `js/`: Responsive styling (including dark mode) and frontend logic.
* `ioc/`: Contains the CloudFormation YAML for the S3 security policy.


