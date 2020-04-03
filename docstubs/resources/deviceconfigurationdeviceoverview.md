---
title: "deviceConfigurationDeviceOverview resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationDeviceOverview resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Update deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-update.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Update the properties of a [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationVersion|Int32||
|conflictCount|Int32||
|errorCount|Int32||
|failedCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdateDateTime|DateTimeOffset||
|notApplicableCount|Int32||
|notApplicablePlatformCount|Int32||
|pendingCount|Int32||
|successCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```

