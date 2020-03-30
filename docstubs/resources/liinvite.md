---
title: "LIInvite resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIInvite resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|invitationSentFromViewer|Boolean||
|pendingInvitationSentFromViewee|[LIInviteDetails](../resources/liinvitedetails.md)||
|viewerCanConnectViewee|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIInvite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIInvite",
  "viewerCanConnectViewee": true,
  "invitationSentFromViewer": true,
  "pendingInvitationSentFromViewee": {
    "@odata.type": "microsoft.graph.LIInviteDetails",
    "invitationId": "String",
    "validationToken": "String"
  }
}
```

