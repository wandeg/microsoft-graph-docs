---
title: "messageRuleActions resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# messageRuleActions resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignCategories|String collection|**TODO: Add Description**|
|copyToFolder|String|**TODO: Add Description**|
|delete|Boolean|**TODO: Add Description**|
|forwardAsAttachmentTo|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|forwardTo|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|markAsRead|Boolean|**TODO: Add Description**|
|markImportance|importance|**TODO: Add Description**. Possible values are: `low`, `normal`, `high`.|
|moveToFolder|String|**TODO: Add Description**|
|permanentDelete|Boolean|**TODO: Add Description**|
|redirectTo|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|stopProcessingRules|Boolean|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.messageRuleActions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messageRuleActions",
  "moveToFolder": "String",
  "copyToFolder": "String",
  "delete": true,
  "permanentDelete": true,
  "markAsRead": true,
  "markImportance": "String",
  "forwardTo": [
    {
      "@odata.type": "microsoft.graph.recipient",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "String",
        "address": "String"
      }
    }
  ],
  "forwardAsAttachmentTo": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "redirectTo": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "assignCategories": [
    "String"
  ],
  "stopProcessingRules": true
}
```

