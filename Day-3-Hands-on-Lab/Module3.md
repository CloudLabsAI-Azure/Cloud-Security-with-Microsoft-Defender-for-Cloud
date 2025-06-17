### Exercise 3: Threat Analysis Using Microsoft Security Copilot (Read-Only)

## Overview:

In this module, you will explore how to use **Microsoft Security Copilot**—both within the Azure portal and through the standalone Security Copilot experience—to analyze threat intelligence, understand your organization’s attack surface, and respond effectively to cyber threats.

> ⚠️ **Note:** Security Copilot uses advanced generative AI models and may incur additional costs depending on the volume of queries and usage duration.

## Estimated Duration: 20–30 Minutes


## Module Mode:

🔒 **Read-only content (no live resources will be deployed)**
or
🧪 **Standalone lab (recommended for hands-on experience)**

> You may choose to run this module in a **read-only simulation mode** or request a **dedicated lab instance** for interactive usage. The standalone lab provides access to pre-configured logs, threat data, and Security Copilot access.

### Lab Objectives:

* Understand the role of Security Copilot in incident response
* Use Security Copilot to analyze attack surface and security events
* Learn how to ask threat-hunting questions in natural language
* Review and export findings for reporting and auditing

### Task 1: Accessing Microsoft Security Copilot in Azure

1. Navigate to the [Azure Portal](https://portal.azure.com) and ensure you are using a subscription where **Microsoft Security Copilot** is enabled.

2. In the search bar, type **Security Copilot**, and click the result.

3. Explore the welcome interface, including:

   * Threat analysis workspace
   * Notebook interface for guided investigation
   * Response suggestions and summaries

### Task 2: Performing Threat Intelligence Queries

1. In the Copilot notebook interface, try queries such as:

   * “List all suspicious login attempts from the past 24 hours”
   * “Summarize open security incidents affecting critical assets”
   * “Correlate alert XYZ123 with MITRE ATT\&CK tactics”

2. Observe:

   * Auto-completion and suggestion support
   * Structured summaries
   * Linked resources (e.g., Sentinel alerts, Defender incidents)

### Task 3: Reviewing External Attack Surface Insights

1. Type:
   `Summarize my organization’s current external attack surface exposure.`

2. Security Copilot will:

   * Query Defender ESAM (if integrated)
   * Present summaries of discovered domains, IPs, shadow assets
   * Highlight exposed services or expired certificates

### Task 4: Guided Remediation

1. Ask:

   * “What actions should I take for the high severity alert on VM-X?”

2. Copilot returns:

   * Recommended remediation steps
   * Scripted responses (e.g., PowerShell commands)
   * References to relevant documentation

### Task 5: Exporting and Reporting

1. Request:

   * “Create a report summarizing this investigation”

2. Download the output in:

   * PDF
   * Word
   * Markdown

> Use this to share threat reports with security managers or auditors.

### Tips for Effective Use

* Use **natural language queries** for simplicity
* Prefix requests with **"summarize," "list," or "recommend"** for clarity
* Leverage **query history** to revisit past investigations

### Summary

By completing this module, you have:

* Explored the Microsoft Security Copilot experience in Azure and standalone mode
* Queried threat intelligence and security alerts using natural language
* Analyzed attack surface data using Defender ESAM integration
* Created and exported automated reports
