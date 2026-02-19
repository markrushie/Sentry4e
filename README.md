# Sentry 4 e-Mail (v1.1)
![Version](https://img.shields.io/badge/version-1.1.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/Status-L3--Forensic--Validated-success)

**Sentry 4 e-Mail** is a forensic-grade email header analysis and infrastructure vetting engine. Developed by **Mark Rushie, MSIS**, this no-code AI solution (deployed via Google Labs) provides a structured methodology for triaging high volumes of professional outreach. By analyzing the "Infrastructure as a Service" (IaaS) footprint of the sender, Sentry protects professional PII from predatory phishing and unverified "ghost" recruiting.

### **Core Capabilities**
* **Deep Infrastructure Vetting:** Beyond basic domain checks, Sentry identifies proxy masking (e.g., `tcpdoor.net`), data center geolocations, and hosting provider reputation.
* **Authentication Governance:** Comprehensive audit of **SPF, DKIM, and DMARC** alignment to verify sender authority.
* **Hop Latency Forensics:** Analyzes server-to-server timestamps to detect relay anomalies or unauthorized interceptions.
* **Algorithmic Credibility Scoring:** A strict 10-point rubric that deducts for high-risk infrastructure patterns and rewards verified enterprise-tenant authenticity.

### **Validation Case Studies (Feb 18, 2026)**
The Sentry logic was subjected to a forensic stress test to validate its scoring consistency:

* **Test Case A (High-Risk/Suspicious):** `jdghd866@seznam.cz` via Paris-based Proxy.
    * **Sentry Verdict: 4/10.**
    * **Forensic Note:** Logic correctly flagged the use of a Czech burner domain paired with a French data center proxy.
* **Test Case B (High-Trust/Verified):** `rajesh.g@fusionplusinc.com` via M365 Enterprise.
    * **Sentry Verdict: 10/10.**
    * **Forensic Note:** Logic successfully validated the Microsoft 365 Enterprise tenant and geographical alignment.

### **Technical Architecture**
* **Engine:** Google Labs (Opal)
* **Logic Framework:** L3 Forensic Analysis Rubric
* **Developer:** Mark Rushie, MSIS

---

### **Support & Enterprise Consulting**
For advanced forensic email audits or enterprise security consulting, contact **service@mrtechnyc.com**.