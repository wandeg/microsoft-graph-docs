---
title: "comanagedDevicesSummary resource type"
description: "Summary data for co managed devices"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# comanagedDevicesSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Summary data for co managed devices

## Properties

| Property                      | Type  | Description                                                                             |
| :---------------------------- | :---- | :-------------------------------------------------------------------------------------- |
| compliancePolicyCount         | Int32 | Number of devices with CompliancePolicy swung-over. This property is read-only.         |
| configurationSettingsCount    | Int32 | Number of devices with ConfigurationSettings swung-over. This property is read-only.    |
| endpointProtectionCount       | Int32 | Number of devices with EndpointProtection swung-over. This property is read-only.       |
| inventoryCount                | Int32 | Number of devices with Inventory swung-over. This property is read-only.                |
| modernAppsCount               | Int32 | Number of devices with ModernApps swung-over. This property is read-only.               |
| officeAppsCount               | Int32 | Number of devices with OfficeApps swung-over. This property is read-only.               |
| resourceAccessCount           | Int32 | Number of devices with ResourceAccess swung-over. This property is read-only.           |
| windowsUpdateForBusinessCount | Int32 | Number of devices with WindowsUpdateForBusiness swung-over. This property is read-only. |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagedDevicesSummary",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.comanagedDevicesSummary",
  "compliancePolicyCount": "Int32",
  "configurationSettingsCount": "Int32",
  "endpointProtectionCount": "Int32",
  "inventoryCount": "Int32",
  "modernAppsCount": "Int32",
  "officeAppsCount": "Int32",
  "resourceAccessCount": "Int32",
  "windowsUpdateForBusinessCount": "Int32"
}
```