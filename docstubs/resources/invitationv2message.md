---
title: "InvitationV2Message resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# InvitationV2Message resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|invitationMessage|[InvitationMessage](../resources/invitationmessage.md)||
|invitationTemplateID|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.InvitationV2Message"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.InvitationV2Message",
  "invitationTemplateID": "String",
  "invitationMessage": {
    "@odata.type": "microsoft.graph.InvitationMessage",
    "body": "String"
  }
}
```

