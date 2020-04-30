---
title: "permissionConditionSet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# permissionConditionSet resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|includeAllPermissions|Boolean|**TODO: Add Description**|
|includeSpecificPermissions|String collection|**TODO: Add Description**|
|resourceApplication|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.permissionConditionSet"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.permissionConditionSet",
  "resourceApplication": "String",
  "includeAllPermissions": true,
  "includeSpecificPermissions": [
    "String"
  ]
}
```

