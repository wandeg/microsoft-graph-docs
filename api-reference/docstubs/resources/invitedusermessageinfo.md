---
title: "invitedUserMessageInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
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
None

## JSON representation
Here is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.recipient",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "String",
        "address": "String"
      }
    }
  ],
  "messageLanguage": "String",
  "customizedMessageBody": "String"
}
```

