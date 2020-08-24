---
title: "configurationManagerClientState enum type"
description: "Configuration manager client state"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# configurationManagerClientState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configuration manager client state

## Members

| Member             | Value | Description                                                                                                                                          |
| :----------------- | ----: | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| unknown            | 0     | Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.                         |
| installed          | 1     | The configuration manager agent is installed but may not be showing up in the configuration manager console yet. Wait a few hours for it to refresh. |
| healthy            | 7     | This device was able to check in with the configuration manager service successfully.                                                                |
| installFailed      | 8     | The configuration manager agent failed to install.                                                                                                   |
| updateFailed       | 11    | The update from version x to version y of the configuration manager agent failed.                                                                    |
| communicationError | 19    | The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.                        |