---
title: "deviceManagementIntentDeviceStateSummary resource type"
description: "Entity that represents device state summary for an intent"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementIntentDeviceStateSummary resource type

Entity that represents device state summary for an intent


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementIntentDeviceStateSummaries](../api/devicemanagementintentdevicestatesummary-list.md)|[deviceManagementIntentDeviceStateSummary](../resources/deviceManagementIntentDeviceStateSummary.md) collection|List properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) objects.|
|[Get deviceManagementIntentDeviceStateSummary](../api/devicemanagementintentdevicestatesummary-get.md)|[deviceManagementIntentDeviceStateSummary](../resources/deviceManagementIntentDeviceStateSummary.md)|Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object.|
|[Create deviceManagementIntentDeviceStateSummary](../api/devicemanagementintentdevicestatesummary-create.md)|[deviceManagementIntentDeviceStateSummary](../resources/deviceManagementIntentDeviceStateSummary.md)|Create a new [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object.|
|[Delete deviceManagementIntentDeviceStateSummary](../api/devicemanagementintentdevicestatesummary-delete.md)|None|Deletes a [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md).|
|[Update deviceManagementIntentDeviceStateSummary](../api/devicemanagementintentdevicestatesummary-update.md)|[deviceManagementIntentDeviceStateSummary](../resources/deviceManagementIntentDeviceStateSummary.md)|Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictCount|Int32|Number of devices in conflict|
|errorCount|Int32|Number of error devices|
|failedCount|Int32|Number of failed devices|
|id|String| Inherited from [entity](../resources/entity.md)|
|notApplicableCount|Int32|Number of not applicable devices|
|notApplicablePlatformCount|Int32|Number of not applicable devices due to mismatch platform and policy|
|successCount|Int32|Number of succeeded devices|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024
}
```

