# Module 2: Securing VMs with Azure Security Baselines

### Task 1: Accessing Microsoft Defender for Cloud

In this task, you will navigate to **Microsoft Defender for Cloud** to begin applying security baselines to your Azure Virtual Machines (VMs).

1. Sign in to the [Azure Portal](https://portal.azure.com).

2. In the top search bar, type **Microsoft Defender** and select **Microsoft Defender for Cloud** from the results.

   ![](./images/M0-T1-S1.2.png)

3. This opens the **Overview** page, showing the security posture of your environment.



### Task 2: Viewing Security Recommendations for VMs

In this task, you will identify and review baseline security recommendations specific to your virtual machines.

1. In the left navigation, click on **Recommendations**.

2. Use the **filter** or **search bar** to locate recommendations related to **Virtual Machines**.

3. Review key recommendations such as:

   * **Enable endpoint protection on virtual machines**
   * **Provision the Log Analytics agent**
   * **Apply system updates**

   ![](./images/task2.1.png)

4. Click on any recommendation to view:

   * Affected VMs
   * Security impact
   * Remediation guidance



### Task 3: Applying Security Baseline Recommendations

In this task, you will apply key baseline settings to improve the security posture of your VMs.

1. Select a recommendation like **"Missing system updates should be installed"**.

2. Click on the affected VM listed.

3. You will be presented with **"Remediate"** or **"Fix"** buttons (if automated remediation is supported).

   ![](./images/task3.1.png)

4. If automation is not available, follow the **manual remediation steps**, such as:

   * Enabling automatic OS updates
   * Installing specific agents (e.g., Dependency, Monitoring, or Vulnerability Assessment agents)

> **Note:** Some security recommendations are implemented using Azure Policy with `DeployIfNotExists` effect, which auto-remediates where possible.



### Task 4: Enabling Just-In-Time (JIT) VM Access

In this task, you will protect your VM against brute force and port scanning attacks by enabling **Just-In-Time (JIT) access**.

1. In **Microsoft Defender for Cloud**, go to **Inventory** and select a virtual machine.

2. Scroll down and click on **Microsoft Defender for Servers** → **Just-In-Time VM Access**.

3. Click **Enable JIT**.

4. Configure:

   * Allowed ports (e.g., 22 for SSH, 3389 for RDP)
   * Allowed source IP ranges
   * Maximum request time (e.g., 1–3 hours)

   ![](./images/task4.1.png)

5. Click **Save** to enforce JIT access on the VM.

> **Note:** When JIT is enabled, ports are closed by default and only opened on request through Defender for Cloud.



### Task 5: Auditing VM Compliance with Security Baselines

In this task, you will evaluate how well your VMs adhere to baseline controls using compliance standards like **Azure Security Benchmark**.

1. From the Defender for Cloud dashboard, click on **Regulatory compliance**.

2. Select **Azure Security Benchmark (v3 or v2)**.

3. Expand the **"Security Controls"** section related to **Compute** or **Virtual Machines**.

4. Review:

   * Passed and failed controls
   * Resource-level compliance state
   * Remediation guidance

   ![](./images/task5.1.png)



### Task 6: Enabling Defender for Servers Plan

To ensure full coverage of VM baselines, you must enable **Microsoft Defender for Servers**, which includes threat protection, endpoint detection, and security baseline enforcement.

1. In **Environment Settings**, select your subscription.

2. Scroll to **Defender Plans** → Enable **Defender for Servers (Plan 2 recommended)**.

3. Click **Save**.

   > **Plan 2** includes additional features such as Vulnerability Assessment, EDR, and File Integrity Monitoring.



### Summary

By completing this guide, you have:

* Identified and remediated baseline security recommendations for VMs
* Enabled Just-In-Time access to reduce attack surface
* Monitored compliance with Azure Security Benchmark
* Activated Defender for Servers for advanced threat protection

These steps collectively harden your virtual machines against common cloud threats using Microsoft’s built-in security baselines.



Let me know if you'd like this in markdown or want a downloadable PDF!
