---
title: "invitedUserMessageInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# invitedUserMessageInfo resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|ccRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|customizedMessageBody|String|**TODO: Add Description**|
|messageLanguage|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.invitedUserMessageInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.invitedUserMessageInfo",
  "ccRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "messageLanguage": "String",
  "customizedMessageBody": "String"
}
```

