
# Exercise 3: Protecting SQL Servers on Azure Virtual Machines

## Overview:

In this lab, you'll learn how to enable Microsoft Defender for SQL on Azure VMs to detect and respond to threats targeting SQL Server workloads.

## Estimated Duration: 30 min

## Lab Objectives: 

In this lab, you will complete the following tasks:

- Task 1: Enable Microsoft Defender for SQL on a VM with SQL Server
- Task 2: Create or Identify a SQL Server VM
- Task 3: Ensure the VM Is Reporting to Defender for Cloud
- Task 4: Verify Defender Is Enabled on the SQL VM
- Task 5: Generate Sample Alert
- Task 6: Review Alerts

### Task 1: Enable Microsoft Defender for SQL on a VM with SQL Server

1. Go to the **Azure Portal**.
2. Search for and open **Microsoft Defender for Cloud**.
3. Under **Environment settings**, click your subscription.
4. Click on **Defender plans**.
5. Ensure **Microsoft Defender for SQL servers on machines** is set to **On**.
6. Click **Save**.

### Task 2: Create or Identify a SQL Server VM

If you already have a VM with SQL Server, skip to Step 3.

**To create one:**

1. Go to **Azure Portal** > **Virtual Machines** > **Create**.
2. In the **Image** dropdown, select a SQL Server-based image like:

   * `SQL Server 2019 on Windows Server 2019`
3. Fill in the required fields (name, region, credentials).
4. Deploy the VM.

### Task 3: Ensure the VM Is Reporting to Defender for Cloud

1. In **Microsoft Defender for Cloud**, under **Inventory**, find your SQL VM.
2. Ensure its **Defender status** is **Healthy** or **Monitored**.
3. If not, ensure the **Log Analytics agent** or **Azure Monitor Agent** is installed.

   * Defender for Cloud auto-installs agents for Azure VMs.

### Task 4: Verify Defender Is Enabled on the SQL VM

1. Go to **Defender for Cloud** > **Inventory**.
2. Select your SQL VM.
3. In the **Security tab**, confirm that **Microsoft Defender for SQL** is enabled.

### Task 5: Generate Sample Alert

To simulate an alert:

* Connect to the VM using **RDP**.
* Open **SQL Server Management Studio (SSMS)**.
* Try running:

    ```sql
    -- Run this multiple times with wrong credentials to simulate brute-force
    -- or simulate an injection query like
    SELECT * FROM Users WHERE username = 'admin' OR 1=1;
    ```

  > ⚠️ These should only be done in a **test environment**. Do **not** simulate attacks in production.

### Task 6: Review Alerts

1. Go back to **Microsoft Defender for Cloud**.
2. Navigate to **Security alerts**.
3. Review alerts related to your SQL VM (if any appear after simulation).


### **Summary:**

By completing this lab, you enabled Microsoft Defender for SQL on Azure VMs to detect and respond to SQL-related threats. This provides real-time threat detection, security alerts, and continuous protection for your SQL workloads.


## You have successfully completed the lab >> Click on Next
