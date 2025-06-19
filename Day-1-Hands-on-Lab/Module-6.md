# **Exercise 6 : Managing VM Access with Just-in-Time (JIT) Access**

## **Objective**

After completing this lab, you will be able to:

* Enable Microsoft Defender for Cloud.
* Configure and verify Just-in-Time (JIT) VM access.
* Secure VM access by restricting public RDP access and enabling access only through JIT.

## **Estimated time**: 30 minutes

### **Task 1: Enable Microsoft Defender for Cloud and JIT Access**

1. In the **Azure portal**, go to **Microsoft Defender for Cloud**.
2. From the **Getting started** page, enable **Enhanced security** and ensure **automatic agent installation** is enabled.

---

### **Task 2: Deploy a Windows VM**

| Setting              | Value                                                    |
| -------------------- | -------------------------------------------------------- |
| Resource group       | **JIT-RG**                                               |
| VM name              | **jitvm01**                                              |
| Region               | Choose a region                                          |
| Image                | **Windows Server 2022 Datacenter: Azure Edition - Gen2** |
| Size                 | Standard\_D2s\_v3                                        |
| Username             | **Student**                                              |
| Password             | **Pa55w\.rd1234**                                        |
| Public inbound ports | None (Important!)                                        |
| Boot diagnostics     | Enable with managed storage                              |

> ⚠️ Ensure no RDP port is exposed during deployment.

---

### **Task 3: Enable Just-in-Time VM Access**

1. In the **Azure portal**, browse to the **Microsoft Defender for Cloud**.
2. Navigate to **Workload protections** > **Just-in-time VM access**.
3. On the **Not Configured** tab, locate your **jitvm01** VM.
4. Select the VM and choose **Enable JIT on 1 VM**.
5. In the JIT configuration pane:

   * Ensure **3389 (RDP)** is listed.
   * Configure allowed IP range (e.g., your current IP).
   * Leave default port settings and click **Save**.

---

### **Task 4: Request JIT Access and Connect via RDP**

1. In **Microsoft Defender for Cloud**, go to **Just-in-time VM access** > **Configured** tab.
2. Select **jitvm01** and click **Request access**.
3. Choose:

   * Port: **3389**
   * Source IP: your current IP
   * Duration: e.g., 1 hour
4. After the request is approved, go to the VM overview page.
5. Use the public IP shown (if not available, assign one via NIC settings) and connect via Remote Desktop using:

   * Username: **Student**
   * Password: **Pa55w\.rd1234**

> ✅ You should now be able to access the VM only because JIT granted access.


## **Result**

You have now enabled Just-in-Time VM access, verified its functionality, and confirmed that access to the VM is only granted when explicitly requested — enhancing your VM’s security posture.
