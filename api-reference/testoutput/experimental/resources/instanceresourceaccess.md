---
title: "instanceResourceAccess resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# instanceResourceAccess resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|permissions|[resourcePermission](../resources/resourcepermission.md) collection||
|resourceAppId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.instanceResourceAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.instanceResourceAccess",
  "resourceAppId": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.resourcePermission",
      "type": "String",
      "value": "String"
    }
  ]
}
```

