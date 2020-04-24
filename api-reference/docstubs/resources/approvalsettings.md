---
title: "approvalSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# approvalSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|approvalMode|String|**TODO: Add Description**|
|approvalStages|[approvalStage](../resources/approvalstage.md) collection|**TODO: Add Description**|
|isApprovalRequired|Boolean|**TODO: Add Description**|
|isApprovalRequiredForExtension|Boolean|**TODO: Add Description**|
|isRequestorJustificationRequired|Boolean|**TODO: Add Description**|

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

