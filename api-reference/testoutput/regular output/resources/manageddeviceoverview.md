---
title: "managedDeviceOverview resource type"
description: "Summary data for managed devices"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedDeviceOverview resource type

Summary data for managed devices


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedDeviceOverviews](../api/manageddeviceoverview-list.md)|[managedDeviceOverview](../resources/managedDeviceOverview.md) collection|List properties and relationships of the [managedDeviceOverview](../resources/manageddeviceoverview.md) objects.|
|[Get managedDeviceOverview](../api/manageddeviceoverview-get.md)|[managedDeviceOverview](../resources/managedDeviceOverview.md)|Read properties and relationships of the [managedDeviceOverview](../resources/manageddeviceoverview.md) object.|
|[Create managedDeviceOverview](../api/manageddeviceoverview-create.md)|[managedDeviceOverview](../resources/managedDeviceOverview.md)|Create a new [managedDeviceOverview](../resources/manageddeviceoverview.md) object.|
|[Delete managedDeviceOverview](../api/manageddeviceoverview-delete.md)|None|Deletes a [managedDeviceOverview](../resources/manageddeviceoverview.md).|
|[Update managedDeviceOverview](../api/manageddeviceoverview-update.md)|[managedDeviceOverview](../resources/managedDeviceOverview.md)|Update the properties of a [managedDeviceOverview](../resources/manageddeviceoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/deviceExchangeAccessStateSummary.md)|Distribution of Exchange Access State in Intune|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/deviceOperatingSystemSummary.md)|Device operating system summary.|
|dualEnrolledDeviceCount|Int32|The number of devices enrolled in both MDM and EAS|
|enrolledDeviceCount|Int32|Total enrolled device count. Does not include PC devices managed via Intune PC Agent|
|id|String| Inherited from [entity](../resources/entity.md)|
|mdmEnrolledCount|Int32|The number of devices enrolled in MDM|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
  }
}
```

