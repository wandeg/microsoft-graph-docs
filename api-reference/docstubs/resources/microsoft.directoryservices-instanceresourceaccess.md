---
title: "instanceResourceAccess resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# instanceResourceAccess resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|permissions|[resourcePermission](../resources/microsoft.directoryservices-resourcepermission.md) collection|**TODO: Add Description**|
|resourceAppId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.instanceResourceAccess"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.instanceResourceAccess",
  "resourceAppId": "String",
  "permissions": [
    {
      "@odata.type": "Microsoft.DirectoryServices.resourcePermission",
      "type": "String",
      "value": "String"
    }
  ]
}
```

