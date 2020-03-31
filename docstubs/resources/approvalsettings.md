---
title: "approvalSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# approvalSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|approvalMode|String||
|approvalStages|[approvalStage](../resources/approvalstage.md) collection||
|isApprovalRequired|Boolean||
|isApprovalRequiredForExtension|Boolean||
|isRequestorJustificationRequired|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.approvalSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalSettings",
  "isApprovalRequired": true,
  "isApprovalRequiredForExtension": true,
  "isRequestorJustificationRequired": true,
  "approvalMode": "String",
  "approvalStages": [
    {
      "@odata.type": "microsoft.graph.approvalStage",
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
  ]
}
```

