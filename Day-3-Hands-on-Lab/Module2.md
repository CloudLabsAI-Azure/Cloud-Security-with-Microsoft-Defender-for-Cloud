# Exercise 2: Deploying and Utilizing Microsoft Defender ESAM in Azure 

## Overview:
In this lab, you will explore how to provision and use Microsoft Defender External Attack Surface Management (ESAM) to gain visibility into your organization's external-facing assets. You will analyze the discovered assets, investigate potential exposures, and take actions to reduce risk—enhancing your organization’s security posture against internet-based threats. 

## Estimated Duration: 45 Minutes

### Task 1: Understanding Microsoft Defender ESAM

Before provisioning, it’s important to understand what **Defender External Surface Attack Management (ESAM)** is.

* **Defender ESAM** provides a comprehensive view of your **external attack surface**, discovering unknown internet-facing assets, shadow IT, exposed services, and misconfigurations.
* It helps identify threats **before** attackers can exploit them, enabling proactive mitigation.



### Task 2: Enabling Microsoft Defender ESAM

In this task, you’ll enable Microsoft Defender ESAM from the Azure portal.

1. Go to [Azure Portal](https://portal.azure.com) and sign in.

2. In the top search bar, type **Microsoft Defender for Cloud** and select it.

   ![](./images/M0-T1-S1.2.png)

3. In the left menu, click **Environment settings**.

4. Select the desired **subscription**.

5. Scroll down to the **Microsoft Defender plans** section.

6. Locate **Defender External Attack Surface Management (ESAM)** and toggle it to **On**.

7. Click **Save**.

   ![](./images/task2.1.png)

> ⚠️ **Note:** ESAM may require additional permissions or a billing-enabled Azure subscription.



### Task 3: Accessing Defender ESAM Dashboard

In this task, you will access the ESAM interface to explore your external attack surface.

1. After enabling, in **Defender for Cloud**, expand the **External Attack Surface Management** option in the left menu.

2. Click **Dashboard** to open the ESAM overview.

3. You will see:

   * Total discovered assets
   * Exposed services
   * Shadow domains
   * Insecure configurations
   * Risk level by asset type

   ![](./images/task3.1.png)



### Task 4: Reviewing Discovered Assets

In this task, you will explore assets that Defender ESAM has discovered.

1. Click on the **Asset inventory** tab.

2. Filter by **asset type**:

   * Domains
   * IP addresses
   * Certificates
   * Cloud services (storage, compute, etc.)

3. Select an asset to view:

   * **Asset metadata**
   * Associated risks
   * Geographic location
   * History of exposure

4. Use **Export** if you want to download the asset list.



### Task 5: Investigating Exposed Services and Risks

In this task, you will analyze risk indicators associated with discovered assets.

1. From the left menu, click **Risks** or select a high-risk asset from the dashboard.

2. Review:

   * Open ports and protocols
   * Expired or weak SSL certificates
   * Insecure DNS records
   * Services with known vulnerabilities

3. Use the **risk priority score** to decide what needs urgent attention.

   ![](./images/task5.1.png)



### Task 6: Taking Action on Vulnerabilities

In this task, you’ll take action to secure your assets based on ESAM’s findings.

1. For any exposed services or high-risk indicators:

   * Click **Remediate**
   * Follow recommended steps (e.g., close ports, renew certificates, remove unused DNS records)

2. You can assign findings to security owners or integrate with ticketing systems via Logic Apps.

3. Regularly review and update configurations to maintain a minimal attack surface.



### Task 7: Setting Up Alerts and Notifications

1. Go to **Settings** > **Notification rules** within the ESAM blade.

2. Add notification rules to receive alerts on:

   * New asset discovery
   * Changes in exposure
   * High-risk vulnerabilities

3. Choose delivery methods:

   * Email
   * Webhook
   * Logic App

### Summary

By completing this lab, you have:

* Enabled **Microsoft Defender ESAM** to monitor your external cloud attack surface
* Explored discovered assets and analyzed associated risks
* Taken remediation actions to secure exposed services
* Configured alerts to stay informed of attack surface changes

## You have successfully completed the lab >> Click on Next
