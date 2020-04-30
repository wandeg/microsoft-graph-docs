---
title: "deviceKey resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# deviceKey resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|Guid|**TODO: Add Description**|
|keyMaterial|Binary|**TODO: Add Description**|
|keyType|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.deviceKey"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.deviceKey",
  "keyType": "String",
  "keyMaterial": "binary",
  "deviceId": "Guid"
}
```

