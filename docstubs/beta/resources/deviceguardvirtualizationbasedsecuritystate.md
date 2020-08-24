---
title: "deviceGuardVirtualizationBasedSecurityState enum type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# deviceGuardVirtualizationBasedSecurityState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Members

| Member                          | Value | Description                                                           |
| :------------------------------ | ----: | :-------------------------------------------------------------------- |
| running                         | 0     | Running                                                               |
| rebootRequired                  | 1     | Root required                                                         |
| require64BitArchitecture        | 2     | 64 bit architecture required                                          |
| notLicensed                     | 3     | Not licensed                                                          |
| notConfigured                   | 4     | Not configured                                                        |
| doesNotMeetHardwareRequirements | 5     | System does not meet hardware requirements                            |
| other                           | 42    | Other. Event logs in microsoft-Windows-DeviceGuard have more details. |