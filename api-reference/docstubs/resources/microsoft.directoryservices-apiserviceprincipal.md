---
title: "apiServicePrincipal resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# apiServicePrincipal resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|resourceSpecificApplicationPermissions|[resourceSpecificPermission](../resources/microsoft.directoryservices-resourcespecificpermission.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.apiServicePrincipal"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.apiServicePrincipal",
  "resourceSpecificApplicationPermissions": [
    {
      "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermission",
      "description": "String",
      "displayName": "String",
      "id": "Guid",
      "isEnabled": true,
      "value": "String"
    }
  ]
}
```

