# Enabling Microsoft defender for cloud for open source rational databases

### Estimated Duration: 45–60 minutes

### Prerequisites:

* Azure subscription (with Owner or Contributor + Security Admin role)
* One of the following databases provisioned:

  * Azure Database for MySQL (Single server or Flexible server)
  * Azure Database for PostgreSQL (Single server or Flexible server)
* Microsoft Defender for Cloud must be enabled in your subscription (at least Free tier)

## Task 1: **Enable Microsoft Defender for Cloud at the Subscription Level**

1. Go to the [Azure Portal](https://portal.azure.com).
2. In the search bar, type **Defender for Cloud**, and select it.
3. In the left pane, click **Environment settings**.
4. Select your **Subscription**.
5. Under **Defender plans**, click **Enable all plans** (or enable only **Databases** plan if preferred).
6. Click **Save**.

  >Note: Enabling Defender for Databases may incur cost. Confirm pricing before proceeding.

## Task 2: **Enable Microsoft Defender for a Specific Open Source Database**

1. In the Azure portal, go to **Resource Groups** and open the resource group containing your database.
2. Select your **Azure Database for MySQL** or **PostgreSQL**.
3. In the database menu, go to **Microsoft Defender for Cloud** (or **Security**).
4. Click **Enable Microsoft Defender for this resource**.
5. Save the configuration.

## Task 3: **Simulate or Wait for Security Insights**

Microsoft Defender for Cloud continuously analyzes your environment. After enabling:

* **Wait for \~30-60 minutes** for the first scan to complete.
* It will evaluate your database configuration, access policies, and data encryption posture.

## Task 4: **Review Security Recommendations for Your Open Source Database**

1. Return to **Microsoft Defender for Cloud**.
2. Click on **Recommendations** from the left-hand pane.
3. Use the **Filter**:

   * **Resource Type**: Choose `Azure Database for PostgreSQL` or `Azure Database for MySQL`
4. Review available recommendations, such as:

   * **Enable SSL connection enforcement**
   * **Enable audit logs**
   * **Restrict public network access**
   * **Enable data encryption at rest**
   * **Configure firewall rules securely**

## Task 5: **Remediate Issues**

1. Click on each recommendation.
2. Review the **Justification** and **Remediation steps**.
3. Apply the suggested settings either via:

   * Azure Portal
   * Azure CLI / PowerShell
   * ARM template

🛠 Example: For "Public network access should be disabled", go to the DB settings → Networking → Disable Public Access.

## Task 6: **Verify Compliance After Fixes**

1. After applying changes, return to Defender for Cloud.
2. Go to **Security Posture** → **Recommendations** again.
3. Check that the status of resolved issues is updated (may take 10–30 minutes).

## 🔍 Optional: Query Alerts and Security Incidents

1. In **Defender for Cloud**, navigate to **Workload Protections** > **Databases**.
2. Check for **Alerts** and **Incidents**.
3. You can integrate these with **Microsoft Sentinel** or a Logic App for alert automation.

## 📘 Additional Tips

* Use **Azure Policy** to enforce secure configurations across all databases.
* Use **Azure Monitor Logs** + **Log Analytics Workspace** for long-term analytics.
* Integrate **Defender for Cloud** with **Security Center API** for automation.

## You have successfully completed the lab >> Click on Next
