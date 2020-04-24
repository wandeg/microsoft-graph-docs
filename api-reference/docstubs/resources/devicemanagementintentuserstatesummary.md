---
title: "deviceManagementIntentUserStateSummary resource type"
description: "Entity that represents user state summary for an intent"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementIntentUserStateSummary resource type


Namespace: microsoft.graph

Entity that represents user state summary for an intent


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentUserStateSummary](../api/devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md)|Read the properties and relationships of a [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) object.|
|[Update deviceManagementIntentUserStateSummary](../api/devicemanagementintentuserstatesummary-update.md)|[deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md)|Update the properties of a [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictCount|Int32|Number of users in conflict|
|errorCount|Int32|Number of error users|
|failedCount|Int32|Number of failed users|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|notApplicableCount|Int32|Number of not applicable users|
|successCount|Int32|Number of succeeded users|

## Relationships
None

## JSON representation
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

