---
title: "approvalStage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# approvalStage resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|approvalStageTimeOutInDays|Int32||
|escalationApprovers|[userSet](../resources/userset.md) collection||
|escalationTimeInMinutes|Int32||
|isApproverJustificationRequired|Boolean||
|isEscalationEnabled|Boolean||
|primaryApprovers|[userSet](../resources/userset.md) collection||

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

