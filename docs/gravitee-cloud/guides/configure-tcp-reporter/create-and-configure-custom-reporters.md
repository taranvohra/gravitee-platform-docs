# Create and configure custom reporters

## Prerequisites

Before creating a custom reporter, ensure you meet the following requirements:

* Enterprise license with Galaxy or Universe tier
* Account-level permissions to manage custom reporters
* TCP endpoint accessible from gateway network
* (Optional) JKS or PFX certificate files for TLS connections

## Creating a Custom Reporter

1. From the **Dashboard**, click **Settings**.
2. From the **Settings** menu, click **Custom Reporters**.
3. Click **Create Custom Reporter**.
4. In the **Name** field, enter a unique name for the reporter. The name must meet the following requirements:

* Must be 2-128 characters.
* Allowed characters: alphanumeric, spaces, hyphens, underscores, and periods.

5. Configure the following connection settings:
6. Enter the destination **Host** (maximum 255 characters, no protocol prefix or path).
7. Enter the **Port** (1-65535).
8. Set the **Connection Timeout** in milliseconds.
9. Set the **Reconnect Attempts**.
10. Set the **Reconnect Interval** in milliseconds.
11. Set the **Retry Timeout** in milliseconds.

<figure><img src="../../.gitbook/assets/gravitee-cloud-custom-reporters-step-06.png" alt="Connection settings form with host, port, connection timeout, reconnect attempts, reconnect interval, and retry timeout fields"><figcaption></figcaption></figure>

6. Link the reporter to one or more gateways. To link the reporter to a Gateway, complete the following sub-steps:
7. Click **Add Gateways**.
8. In the **Select Gateways to link** pop-up window, select the Gateways that you want to link to the reporter.
9. Click **Add Gateway**.
10. (Optional) Enable TLS:
11. Toggle **TLS Enabled**.
12. (Optional) Enable **TLS Verify Client** to validate the remote server's certificate.
13. Select the **Keystore Type** (JKS or PFX).
14. Upload the keystore file (maximum 2 MB).
15. Provide the encrypted keystore password.
16. Select the **Truststore Type** (JKS or PFX).
17. Upload the truststore file (maximum 2 MB).
18. Provide the encrypted truststore password.
19. From the **Data Selection** menu, select at least one data type to export from the available options.
20. Click **Save**.

<figure><img src="../../.gitbook/assets/gravitee-cloud-custom-reporters-step-04.png" alt="Edit custom reporter page showing basic configuration, gateway linking, connection settings, TLS configuration, and data selection sections"><figcaption></figcaption></figure>

## Verification

Your Custom Reporter appears in the Custom Reporters screen.
