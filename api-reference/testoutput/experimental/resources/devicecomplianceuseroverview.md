---
title: "deviceComplianceUserOverview resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceUserOverview resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceComplianceUserOverviews](../api/devicecomplianceuseroverview-list.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) collection|List properties and relationships of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) objects.|
|[Get deviceComplianceUserOverview](../api/devicecomplianceuseroverview-get.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Read properties and relationships of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[Create deviceComplianceUserOverview](../api/devicecomplianceuseroverview-create.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Create a new [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[Delete deviceComplianceUserOverview](../api/devicecomplianceuseroverview-delete.md)|None|Deletes a [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md).|
|[Update deviceComplianceUserOverview](../api/devicecomplianceuseroverview-update.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Update the properties of a [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationVersion|Int32|Version of the policy for that overview|
|conflictCount|Int32|Number of users in conflict|
|errorCount|Int32|Number of error Users|
|failedCount|Int32|Number of failed Users|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdateDateTime|DateTimeOffset|Last update time|
|notApplicableCount|Int32|Number of not applicable users|
|pendingCount|Int32|Number of pending Users|
|successCount|Int32|Number of succeeded Users|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```

