# Exercise 1: Enhancing Compliance with Defender for Cloud 

## Overview:
In this exercise, you will learn how to assess and improve the regulatory compliance of your Azure environment using Microsoft Defender for Cloud. You'll explore built-in compliance standards like Azure Security Benchmark, ISO 27001, and more. You’ll review compliance controls, take remediation actions, enable continuous export, and track your compliance score over time.

## Estimated Duration: 45 Minutes

## Lab Objectives:

By the end of this lab, you will be able to:

- Task 1: Accessing Microsoft Defender for Cloud
- Task 2: Navigating to Regulatory Compliance Dashboard
- Task 3: Reviewing Compliance Controls and Assessments
- Task 4: Implementing Remediation Actions
- Task 5: Enabling Auto-Remediation and Continuous Export
- Task 6: Tracking Compliance Over Time

### Task 1: Accessing Microsoft Defender for Cloud

In this task, you will open Microsoft Defender for Cloud to begin checking the compliance status of your Azure resources.

1. Open [https://portal.azure.com](https://portal.azure.com) and sign in with your Azure credentials.

2. In the search bar at the top, type **Microsoft Defender** and select **Microsoft Defender for Cloud** from the results.

3. This will open the **Overview** dashboard for Microsoft Defender for Cloud, where you can view the overall security posture and regulatory compliance status of your environment.

### Task 2: Navigating to Regulatory Compliance Dashboard

In this task, you will access the **Regulatory compliance** section, which provides an overview of how your resources align with industry standards.

1. From the **Defender for Cloud** left-hand navigation pane, click on **Regulatory compliance** under the **Cloud security** section.

2. The dashboard shows a list of supported **compliance standards** such as:

   * Azure Security Benchmark (Default)
   * ISO 27001
   * NIST SP 800-53
   * PCI DSS

3. Each standard displays a **compliance score** and a summary of **passed** and **failed** assessments.

### Task 3: Reviewing Compliance Controls and Assessments

In this task, you will review detailed compliance controls and how each Azure resource aligns with them.

1. Click on a compliance standard (e.g., **Azure Security Benchmark**).

2. The page displays a list of **controls** (e.g., “Secure management ports”, “Enable monitoring”).

3. Each control includes:

   * **Assessment name**
   * **Compliance state** (Healthy, Unhealthy, Not applicable)
   * **Number of resources evaluated**

4. Click on a specific **control** to see:

   * A list of affected resources
   * The **description** of the control
   * **Remediation steps** and impact

### Task 4: Implementing Remediation Actions

In this task, you will take action to remediate non-compliant resources using recommendations provided by Defender for Cloud.

1. Click on a **non-compliant control** to view the affected resources.

2. Each listed resource will show the issue and provide a **“Fix”** or **“View remediation steps”** button.

3. You can:

   * Apply the fix directly (if available)
   * Use the PowerShell/CLI/script provided in the remediation guidance
   * Manually update the resource configuration in Azure

   > **Note:** Some remediations may require elevated privileges (e.g., Contributor or Owner role) to perform changes on resources.

### Task 5: Enabling Auto-Remediation and Continuous Export

In this task, you will configure automatic handling and reporting of compliance issues.

1. In **Microsoft Defender for Cloud**, go to **Environment settings**.

2. Select your subscription and click on the **Continuous export** tab.

3. Choose where to send compliance data (e.g., Log Analytics, Event Hub, Storage Account).

4. Enable **auto-export** of:

   * Regulatory compliance data
   * Security recommendations

   > **Tip:** Exporting compliance data helps integrate with external SIEM or audit systems.

### Task 6: Tracking Compliance Over Time

In this task, you will use the dashboard and reports to monitor compliance progress over time.

1. Return to the **Regulatory compliance** blade.

2. Review the **Compliance score trend** to track improvements or regressions over time.

3. Use filters to view data by:

   * Subscription
   * Resource type
   * Compliance standard

4. Download the compliance reports in CSV or PDF format for documentation or audit reviews.

### Summary

By completing this guide, you have:

* Explored Microsoft Defender for Cloud’s regulatory compliance features
* Identified misconfigured or non-compliant Azure resources
* Taken steps to remediate security issues using guided recommendations
* Enabled continuous export for compliance reporting and audit tracking

## You have successfully completed the lab >> Click on Next