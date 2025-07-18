# Splunk Universal Forwarder: deploymentclient.conf

This file defines the configuration used by a Splunk Universal Forwarder to connect to a central Splunk Deployment Server.

---

## File Path (on endpoint)

C:\Program Files\SplunkUniversalForwarder\etc\system\local\deploymentclient.conf


---

##  Sample Configuration

```ini
[deployment-client]
clientName = WIN-1T5RE39Q2K5

[target-broker:deploymentServer]
targetUri = 127.0.0.1:8089
```
| Setting      | Description                                                                   |
| ------------ | ----------------------------------------------------------------------------- |
| `clientName` | (Optional) Custom name to identify this forwarder in the deployment server    |
| `targetUri`  | IP address or hostname of the Splunk Deployment Server (default port is 8089) |

## Notes
This file must be placed under the local directory to take effect.

## After modifying this file, restart the Splunk Forwarder:

```ini
Restart-Service splunkforwarder
```
## Reference
Splunk Docs: deploymentclient.conf
