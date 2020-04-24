---
title: "approvalStage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# approvalStage resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|approvalStageTimeOutInDays|Int32|**TODO: Add Description**|
|escalationApprovers|[userSet](../resources/userset.md) collection|**TODO: Add Description**|
|escalationTimeInMinutes|Int32|**TODO: Add Description**|
|isApproverJustificationRequired|Boolean|**TODO: Add Description**|
|isEscalationEnabled|Boolean|**TODO: Add Description**|
|primaryApprovers|[userSet](../resources/userset.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.approvalStage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalStage",
  "approvalStageTimeOutInDays": 1024,
  "isApproverJustificationRequired": true,
  "isEscalationEnabled": true,
  "escalationTimeInMinutes": 1024,
  "primaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser",
      "isBackup": true,
      "id": "String",
      "description": "String"
    }
  ],
  "escalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```

