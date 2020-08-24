---
title: "managedDeviceOverview resource type"
description: "Summary data for managed devices"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# managedDeviceOverview resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Summary data for managed devices

## Methods

| Method                                                                        | Return Type                                                         | Description                                                          |
| :---------------------------------------------------------------------------- | :------------------------------------------------------------------ | :------------------------------------------------------------------- |
| [List managedDeviceOverview](../api/intune-manageddeviceoverview-list.md)     | [managedDeviceOverview](intune-managedDeviceOverview.md) collection | List properties and relationships of a managedDeviceOverview object. |
| [Create managedDeviceOverview](../api/intune-manageddeviceoverview-create.md) | [managedDeviceOverview](intune-managedDeviceOverview.md)            | Create a new managedDeviceOverview object.                           |
| [Get managedDeviceOverview](../api/intune-manageddeviceoverview-get.md)       | [managedDeviceOverview](intune-managedDeviceOverview.md)            | Read properties and relationships of a managedDeviceOverview object. |
| [Update managedDeviceOverview](../api/intune-manageddeviceoverview-update.md) | [managedDeviceOverview](intune-managedDeviceOverview.md)            | Update the properties of a managedDeviceOverview object.             |
| [Delete managedDeviceOverview](../api/intune-manageddeviceoverview-delete.md) |                                                                     | Delete a managedDeviceOverview object.                               |

## Properties

| Property                            | Type                                                                                       | Description                                                                          |
| :---------------------------------- | :----------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------- |
| deviceExchangeAccessStateSummary    | [deviceExchangeAccessStateSummary](../resources/deviceexchangeaccessstatesummary.md)       | Distribution of Exchange Access State in Intune                                      |
| deviceOperatingSystemSummary        | [deviceOperatingSystemSummary](../resources/deviceoperatingsystemsummary.md)               | Device operating system summary.                                                     |
| dualEnrolledDeviceCount             | Int32                                                                                      | The number of devices enrolled in both MDM and EAS                                   |
| enrolledDeviceCount                 | Int32                                                                                      | Total enrolled device count. Does not include PC devices managed via Intune PC Agent |
| id                                  | String                                                                                     | Unique Identifier for the summary Read-only.                                         |
| lastModifiedDateTime                | DateTimeOffset                                                                             | Last modified date time of device overview                                           |
| managedDeviceModelsAndManufacturers | [managedDeviceModelsAndManufacturers](../resources/manageddevicemodelsandmanufacturers.md) | Models and Manufactures meatadata for managed devices in the account                 |
| mdmEnrolledCount                    | Int32                                                                                      | The number of devices enrolled in MDM                                                |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "deviceExchangeAccessStateSummary": {"@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"},
  "deviceOperatingSystemSummary": {"@odata.type": "microsoft.graph.deviceOperatingSystemSummary"},
  "dualEnrolledDeviceCount": "Int32",
  "enrolledDeviceCount": "Int32",
  "id": "String (identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "managedDeviceModelsAndManufacturers": {"@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"},
  "mdmEnrolledCount": "Int32"
}
```