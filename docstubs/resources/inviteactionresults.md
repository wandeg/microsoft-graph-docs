---
title: "InviteActionResults resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# InviteActionResults resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|inviteActionResults|[InviteActionStatus](../resources/inviteactionstatus.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.InviteActionResults"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.InviteActionResults",
  "inviteActionResults": [
    {
      "@odata.type": "microsoft.graph.InviteActionStatus",
      "id": "String",
      "status": 1024,
      "message": "String"
    }
  ]
}
```

