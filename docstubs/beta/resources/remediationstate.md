---
title: "remediationState enum type"
description: "Indicates the type of execution status of the device management script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# remediationState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indicates the type of execution status of the device management script.

## Members

| Member            | Value | Description                                                                        |
| :---------------- | ----: | :--------------------------------------------------------------------------------- |
| unknown           | 0     | Unknown result.                                                                    |
| skipped           | 1     | Remediation script execution was skipped                                           |
| success           | 2     | Remediation script executed successfully and remediated the device state           |
| remediationFailed | 3     | Remediation script executed successfully but failed to remediated the device state |
| scriptError       | 4     | Remediation script execution encountered and error or timed out                    |