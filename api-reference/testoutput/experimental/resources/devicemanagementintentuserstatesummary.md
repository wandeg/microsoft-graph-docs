---
title: "deviceManagementIntentUserStateSummary resource type"
description: "Entity that represents user state summary for an intent"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementIntentUserStateSummary resource type

Entity that represents user state summary for an intent


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementIntentUserStateSummaries](../api/devicemanagementintentuserstatesummary-list.md)|[deviceManagementIntentUserStateSummary](../resources/deviceManagementIntentUserStateSummary.md) collection|List properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) objects.|
|[Get deviceManagementIntentUserStateSummary](../api/devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/deviceManagementIntentUserStateSummary.md)|Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) object.|
|[Create deviceManagementIntentUserStateSummary](../api/devicemanagementintentuserstatesummary-create.md)|[deviceManagementIntentUserStateSummary](../resources/deviceManagementIntentUserStateSummary.md)|Create a new [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) object.|
|[Delete deviceManagementIntentUserStateSummary](../api/devicemanagementintentuserstatesummary-delete.md)|None|Deletes a [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md).|
|[Update deviceManagementIntentUserStateSummary](../api/devicemanagementintentuserstatesummary-update.md)|[deviceManagementIntentUserStateSummary](../resources/deviceManagementIntentUserStateSummary.md)|Update the properties of a [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictCount|Int32|Number of users in conflict|
|errorCount|Int32|Number of error users|
|failedCount|Int32|Number of failed users|
|id|String| Inherited from [entity](../resources/entity.md)|
|notApplicableCount|Int32|Number of not applicable users|
|successCount|Int32|Number of succeeded users|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```

