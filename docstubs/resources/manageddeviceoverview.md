---
title: "managedDeviceOverview resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDeviceOverview resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDeviceOverview](../api/manageddeviceoverview-get.md)|[managedDeviceOverview](../resources/manageddeviceoverview.md)|Read properties and relationships of the [managedDeviceOverview](../resources/manageddeviceoverview.md) object.|
|[Update managedDeviceOverview](../api/manageddeviceoverview-update.md)|[managedDeviceOverview](../resources/manageddeviceoverview.md)|Update the properties of a [managedDeviceOverview](../resources/manageddeviceoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/deviceexchangeaccessstatesummary.md)||
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/deviceoperatingsystemsummary.md)||
|dualEnrolledDeviceCount|Int32||
|enrolledDeviceCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|managedDeviceModelsAndManufacturers|[managedDeviceModelsAndManufacturers](../resources/manageddevicemodelsandmanufacturers.md)||
|mdmEnrolledCount|Int32||

## Relationships
None

## JSON representation
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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

