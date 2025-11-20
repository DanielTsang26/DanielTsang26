

# 🛡️ Security Technical Implementation Guides (STIGs) — Overview for Windows 11

## 📘 What Are STIGs?

**Security Technical Implementation Guides (STIGs)** are standardized cybersecurity configuration guidelines developed by the **Defense Information Systems Agency (DISA)**. They define the security controls, configuration requirements, and hardening standards necessary to protect systems used within U.S. Department of Defense (DoD) environments.

STIGs establish a baseline of secure configurations that reduce attack surface and ensure systems meet **DoD-level compliance**. Even outside military use, organizations adopt STIGs to strengthen security posture, reduce risk, and enforce consistent, hardened configurations across Windows systems.

---

# 🔐 Why STIGs Matter

Implementing STIGs provides:

### **1. Proven Security Hardening**

STIGs are rigorously vetted and represent industry-leading standards for secure configuration. They directly target:

* Misconfigurations
* Unnecessary services
* Vulnerable settings
* Privilege misuse
* Weak authentication or auditing controls

### **2. Reduced Attack Surface**

They force the system into a “minimum viable exposure” configuration—disabling legacy components, enforcing least privilege, enabling structured logging, and restricting access pathways commonly exploited in intrusions.

### **3. Consistent Compliance**

STIGs bring uniformity. Every system that follows the STIG starts from the same hardened baseline, simplifying:

* Security audits
* Vulnerability assessments
* Incident response
* System deployment

### **4. Alignment with Zero Trust Principles**

STIG configurations support modern Zero Trust architectures through strict identity, logging, and system-hardening requirements.

---

# 🪟 Windows 11 STIGs

The **Windows 11 STIG** provides security requirements for modern Windows desktop environments, covering:

### **System Configuration**

* Account policies and password complexity
* UAC elevation controls
* Credential Guard & virtualization-based security
* Restriction of legacy protocols (SMBv1, NTLM fallback, etc.)

### **Auditing & Logging**

* Enhanced Event Log configurations
* Required auditing categories
* Log size and retention requirements
* Ensuring logs cannot be overwritten without review

### **Network Security**

* Firewall rulesets
* Secure communication protocols
* Enforcement of TLS, IPsec, and secure channel protections

### **Application Control**

* SmartScreen
* Controlled Folder Access
* AppLocker or WDAC policies
* Restrictions on unsigned scripts or executables

### **System Services**

* Disabling unnecessary or insecure services
* Locking down remote administration pathways
* Ensuring patching + update configurations are compliant

---

# ⚙️ STIG Severity Levels

STIG findings fall under three severities:

| Severity                 | Description                                                                     |
| ------------------------ | ------------------------------------------------------------------------------- |
| **Category I (High)**    | Immediate mission-critical risk; typically exploited quickly.                   |
| **Category II (Medium)** | Potential for degradation of security posture but not immediately catastrophic. |
| **Category III (Low)**   | Optimization/security hygiene issues that still need correction.                |

---

# 🔧 STIG Remediations in This Repository

This repository implements **Windows 11 STIG-aligned remediations**, including:

* Secure registry configurations
* Hardened local policies
* Audit and logging enhancements
* Firewall and network hardening
* PowerShell-driven automation for compliance
* Documentation for applying and reverting changes

Scripts and configurations are written to be:

* **Idempotent** (safe to rerun)
* **Documented** for clarity
* **Modular** for selective deployment
* **Compatible with Windows 11 / PowerShell 7+**

---

# ✔️ Who Uses STIGs?

* DoD agencies
* Federal organizations
* Defense contractors
* Cybersecurity teams building hardened baselines
* Blue teams developing secure workstation images
* Anyone seeking highly secure configurations

Even outside government environments, STIGs are a **gold standard** for serious Windows hardening.

---

# 📄 References

* DISA STIGs official site
* Microsoft security baselines (Windows 11 / MDM / GPO)
* NIST SP 800-53 + 800-171 alignment



