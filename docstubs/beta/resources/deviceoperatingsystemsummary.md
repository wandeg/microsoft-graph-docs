---
title: "deviceOperatingSystemSummary resource type"
description: "Device operating system summary."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceOperatingSystemSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device operating system summary.

## Properties

| Property                         | Type  | Description                                                                                                                                 |
| :------------------------------- | :---- | :------------------------------------------------------------------------------------------------------------------------------------------ |
| androidCorporateWorkProfileCount | Int32 | The count of Corporate work profile Android devices. Also known as Corporate Owned Personally Enabled (COPE). Valid values -1 to 2147483647 |
| androidCount                     | Int32 | Number of android device count.                                                                                                             |
| androidDedicatedCount            | Int32 | Number of dedicated Android devices.                                                                                                        |
| androidDeviceAdminCount          | Int32 | Number of device admin Android devices.                                                                                                     |
| androidFullyManagedCount         | Int32 | Number of fully managed Android devices.                                                                                                    |
| androidWorkProfileCount          | Int32 | Number of work profile Android devices.                                                                                                     |
| configMgrDeviceCount             | Int32 | Number of ConfigMgr managed devices.                                                                                                        |
| iosCount                         | Int32 | Number of iOS device count.                                                                                                                 |
| macOSCount                       | Int32 | Number of Mac OS X device count.                                                                                                            |
| unknownCount                     | Int32 | Number of unknown device count.                                                                                                             |
| windowsCount                     | Int32 | Number of Windows device count.                                                                                                             |
| windowsMobileCount               | Int32 | Number of Windows mobile device count.                                                                                                      |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCorporateWorkProfileCount": "Int32",
  "androidCount": "Int32",
  "androidDedicatedCount": "Int32",
  "androidDeviceAdminCount": "Int32",
  "androidFullyManagedCount": "Int32",
  "androidWorkProfileCount": "Int32",
  "configMgrDeviceCount": "Int32",
  "iosCount": "Int32",
  "macOSCount": "Int32",
  "unknownCount": "Int32",
  "windowsCount": "Int32",
  "windowsMobileCount": "Int32"
}
```