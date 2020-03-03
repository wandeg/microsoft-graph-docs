---
title: "invitedUserMessageInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# invitedUserMessageInfo resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|ccRecipients|[recipient](../resources/recipient.md) collection||
|customizedMessageBody|String||
|messageLanguage|String||

## Relationships
None

## JSON Representation
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

