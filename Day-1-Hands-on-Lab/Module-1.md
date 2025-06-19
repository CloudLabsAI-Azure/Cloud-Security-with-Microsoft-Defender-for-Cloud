# Exercise 1: Getting Started with Microsoft Defender for Cloud

## Lab Objectives

 In this lab, you will perform the following:
- Task 1: Enable Microsoft Defender for Cloud
- Task 2: Understanding the Microsoft Defender for Cloud Dashboard

### Estimated Timing: 25 minutes

## Architecture Diagram

  ![Picture 1](../Media/Mod5_L1_Ex1.png)

### Task 1: Enable Microsoft Defender for Cloud

In this task, you'll enable and configure Microsoft Defender for Cloud.

1. In the Search bar of the Microsoft Azure portal, type **Defender for Cloud (1)**, then select **Microsoft Defender for Cloud (2)**.

   ![Picture 1](../Media/lab5-8.png)

1. In the left navigation menu for Microsoft Defender for Cloud, expand the *Management* section , and select **Environment settings**.

   ![Picture 1](../Media/lab5-9.png)

1. Select the **Expand all** button to view all subscriptions and resources.

1. Select the your subscription (or equivalent name in your Language).

   ![Picture 1](../Media/lab5-3.png)

1. Review the Azure resources that are now protected with the Defender for Cloud plans.

    >**Important:** If all Defender plans are *Off*, click **Enable all plans**. Then, select the *$200/month Microsoft Defender for APIs Plan 1* and click **Save**. Finally, click **Save** again at the top of the page and wait for the notification *"Defender plans (for your) subscription were saved successfully!"* to appear.

1. Review the **Azure resources** that are currently protected under the **Defender for Cloud plans**.

1. In the **Cloud Security Posture Management (CSPM)** section, set **Defender CSPM** to **On (1)**.

   ![Picture 1](../Media/lab5y1.png)

1. In the **Cloud Workload Protection (CWP)** section, set **Servers Plan 2 (2)** to **On (3)**.

1. Click the **Save (4)** button at the top of the page.

1. Select the **Settings & monitoring** tab from the Settings area (next to Save).

   ![Picture 1](../Media/lab5-10.png)

1. Review the monitoring extensions. It includes configurations for **Virtual Machines, Containers, and Storage Accounts**.

1. Close the "Settings & monitoring" page by selecting the **X** on the upper right of the page.

   ![Picture 1](../Media/lab5-11.png)

1. Close the settings page by selecting the 'X' on the upper right of the page to go back to the **Environment settings**.

### Task 2: Understanding the Microsoft Defender for Cloud Dashboard

In this task, you will explore the Microsoft Defender for Cloud dashboard to familiarize yourself with its interface, features, and how it provides insights into your cloud environment's security posture.

1. In the Search bar of the Microsoft Azure portal, type **Defender for Cloud (1)**, then select **Microsoft Defender for Cloud (2)**.

   ![Picture 1](../Media/lab5-8.png)

1. In the left navigation menu for Microsoft Defender for Cloud, under the *General* section, select **Overview**.

   ![Picture 1](../Media/lab5-12.png)

1. The **Overview blade** offers a unified view of the **security posture** and includes multiple independent **cloud security pillars**, such as **Security posture**, **Regulatory compliance**, **Workload protections**, **Firewall Manager**, **Inventory**, and **Information Protection (preview)**. Each pillar also has its own dedicated dashboard, providing **deeper insights** and **actions** for that area, ensuring **easy access** and **better visibility** for security professionals.

    >**Note:** The top menu bar features a **Subscriptions** button, enabling you to view and filter subscriptions; in this lab, we will use just one subscription, but selecting different or additional subscriptions will update the interface to reflect the **security posture** of the selected subscriptions.

1. Click on the **What’s new** icon link – a new tab opens with the latest release notes where you can stay current on the new features, bug fixes, and more.

    ![Picture 1](../Media/lab5-13.png)

    >**Note:** The high-level numbers in the top menu provide a summary of your subscriptions, active recommendations, security alerts, and connected cloud accounts.

1. From the top menu bar, select **Azure subscriptions**. This will bring you into the environment settings where you can select from the available subscriptions.

   ![Picture 1](../Media/lab5-14.png)

1. Return to the **Overview** page, and review the **Security posture** tile. You can see your current **Secure score** along with the number of completed controls and recommendations. Selecting this tile will redirect you to a drill-down view across subscriptions.

1. On the **Regulatory compliance** tile, you can gain insights into your compliance posture through the continuous assessment of both **Azure** and **hybrid cloud environments**. This tile displays standards such as the **Microsoft Cloud Security benchmark** and the **Lowest compliance regulatory standard**. To view the data, you must first add **Security policies**.

   ![Picture 1](../Media/lab5-16.png)

1. Selecting this tile will redirect you to the **Regulatory compliance** dashboard – where you can add additional standards and explore the current ones.

1. We will continue exploring *Microsoft Defender for Cloud* **Security posture** and **Regulatory compliance** in the next exercise.


## Review

In this lab, you have completed the following:

- Enabled Microsoft Defender for Cloud
- Explored the Microsoft Defender for Cloud Dashboard

## Select **Next** to continue to Lab 2