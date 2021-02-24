# Azure Log Analytics Output Plugin

This plugin sends metrics in a Azure Log Analytics.

## Configuration

```toml
# A plugin that can transmit metrics over HTTP
[[outputs.azure_monitor_logs]]
  ## Customer ID (Workstation ID) and Key for Azure Log Analytics resource.
  # customer_id = "<Workstation ID>"
  # shared_key = "<Secret>"

  ## Timeout for closing (default: 5s).
  # timeout = "5s"

  ## Table Namespace Prefix (default: "").
  ## Namespace Prefix is used in "Log-Type" header
  ## Limited to 25 chars as not to exceed the max limit
  ## Prefix can only contain alphaNumeric characters
  # namespace_prefix = ""
```