---
title: "apiServicePrincipal resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# apiServicePrincipal resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|resourceSpecificApplicationPermissions|[resourceSpecificPermission](../resources/resourcespecificpermission.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiServicePrincipal"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.apiServicePrincipal",
  "resourceSpecificApplicationPermissions": [
    {
      "@odata.type": "microsoft.graph.resourceSpecificPermission",
      "description": "String",
      "displayName": "String",
      "id": "Guid",
      "isEnabled": true,
      "value": "String"
    }
  ]
}
```

