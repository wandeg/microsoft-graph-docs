---
title: "keyCredential resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# keyCredential resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|customKeyIdentifier|Binary|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|key|Binary|**TODO: Add Description**|
|keyId|Guid|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|usage|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.keyCredential"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.keyCredential",
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "type": "String",
  "usage": "String",
  "key": "binary",
  "displayName": "String"
}
```

