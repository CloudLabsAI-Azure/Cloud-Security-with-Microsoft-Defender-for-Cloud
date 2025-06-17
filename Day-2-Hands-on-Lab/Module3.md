# Exercise 3: Investigating and Responding to Security Alerts

### Task 1: Accessing Security Alerts in Microsoft Defender for Cloud

In this task, you will learn how to locate and review security alerts that Defender for Cloud generates when it detects suspicious activities or threats.

1. Go to the [Azure Portal](https://portal.azure.com) and sign in.

2. In the top search bar, type **Microsoft Defender for Cloud** and select it from the results.

   ![](./images/M0-T1-S1.2.png)

3. In the **Microsoft Defender for Cloud** dashboard, click on **Security alerts** from the left-hand navigation menu.

   ![](./images/task1.1.png)

4. This opens a list of alerts categorized by severity:

   * **High** – Immediate action required
   * **Medium** – Review recommended
   * **Low** – Informational or best practices



### Task 2: Filtering and Reviewing a Specific Alert

In this task, you will filter and select an alert for investigation.

1. Use the **Filters** option to search by:

   * Severity (High, Medium, Low)
   * Time range
   * Environment (e.g., subscription or resource group)

2. Select a **High-severity alert** such as:

   * “Suspected crypto mining activity”
   * “Brute-force attack detected”

3. Click on the alert name to view its **details**.

   ![](./images/task2.1.png)



### Task 3: Investigating the Alert Details

In this task, you will analyze the context of the selected alert to understand the scope of the issue.

1. Review the **alert details** page, which provides:

   * **Alert name and description**
   * **Resource impacted** (e.g., VM, Key Vault, Storage)
   * **Time detected**
   * **Entities involved** (IP addresses, users, etc.)
   * **Investigation steps**
   * **Recommended remediation**

2. Use the **Take action** section to follow guided remediation steps or export data for further analysis.

   ![](./images/task3.1.png)



### Task 4: Triggering Investigation in Microsoft Sentinel (Optional)

In this task, if Microsoft Sentinel is connected, you can extend the investigation using its deeper analytics and investigation tools.

1. On the alert page, look for the **“Investigate in Microsoft Sentinel”** link (if integrated).

2. Click to open the **incident** in Sentinel.

3. Use **Entity behavior**, **Timeline**, and **Graph view** to track threat paths and lateral movements.

   ![](./images/task4.1.png)

> **Note:** Sentinel integration is optional but enhances threat investigation significantly through AI-assisted correlation and hunting capabilities.



### Task 5: Responding to the Alert

In this task, you will take remediation actions based on Defender for Cloud recommendations.

1. Based on the alert, take action such as:

   * **Isolate the affected VM**
   * **Reset compromised credentials**
   * **Remove malicious extensions**
   * **Apply missing security updates**

2. If Defender for Cloud offers **automated remediation**, click on the **“Remediate”** button.

3. Document the actions taken for audit and future learning.

> **Tip:** Assign the alert to an analyst or track it via a **ticketing system** if connected through Logic Apps or Sentinel playbooks.

### Task 6: Suppressing or Dismissing Alerts (If Needed)

In this task, you will manage alert noise and false positives.

1. If the alert is a known false positive or non-critical, click **Dismiss alert**.

2. Optionally, use **Suppression rules** to prevent future identical alerts by:

   * Resource ID
   * Alert type
   * Source

   ![](./images/task6.1.png)

> **Caution:** Only suppress alerts when you're certain they are benign to avoid missing real threats.

### Task 7: Enabling Email Notifications for Alerts

In this task, you’ll configure alert forwarding to email or webhook.

1. Go to **Defender for Cloud** > **Environment settings** > Choose your subscription.

2. Click on **Email notifications**.

3. Add email addresses for security admins or response teams.

4. Save the configuration.

> **Bonus:** You can also use **Logic Apps** to send alerts to ticketing systems (e.g., ServiceNow, Jira).

### Summary

By completing this guide, you have:

* Identified and investigated real-time security alerts
* Reviewed alert details to understand their scope and impact
* Taken action to remediate security threats
* Configured alert forwarding and optional Sentinel integration

## You have successfully completed the lab >> Click on Next
