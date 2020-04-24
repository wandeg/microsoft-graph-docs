---
title: "alertHistoryState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# alertHistoryState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String|**TODO: Add Description**|
|assignedTo|String|**TODO: Add Description**|
|comments|String collection|**TODO: Add Description**|
|feedback|alertFeedback|**TODO: Add Description**. Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`, `unknownFutureValue`.|
|status|alertStatus|**TODO: Add Description**. Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`, `unknownFutureValue`.|
|updatedDateTime|DateTimeOffset|**TODO: Add Description**|
|user|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alertHistoryState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.alertHistoryState",
  "appId": "String",
  "assignedTo": "String",
  "comments": [
    "String"
  ],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

