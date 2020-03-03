---
title: "deviceComplianceDeviceOverview resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceComplianceDeviceOverview resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceComplianceDeviceOverviews](../api/devicecompliancedeviceoverview-list.md)|[deviceComplianceDeviceOverview](../resources/deviceComplianceDeviceOverview.md) collection|List properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) objects.|
|[Get deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/deviceComplianceDeviceOverview.md)|Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[Create deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-create.md)|[deviceComplianceDeviceOverview](../resources/deviceComplianceDeviceOverview.md)|Create a new [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[Delete deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-delete.md)|None|Deletes a [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md).|
|[Update deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-update.md)|[deviceComplianceDeviceOverview](../resources/deviceComplianceDeviceOverview.md)|Update the properties of a [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationVersion|Int32|Version of the policy for that overview|
|conflictCount|Int32|Number of devices in conflict|
|errorCount|Int32|Number of error devices|
|failedCount|Int32|Number of failed devices|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdateDateTime|DateTimeOffset|Last update time|
|notApplicableCount|Int32|Number of not applicable devices|
|notApplicablePlatformCount|Int32|Number of not applicable devices due to mismatch platform and policy|
|pendingCount|Int32|Number of pending devices|
|successCount|Int32|Number of succeeded devices|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
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

