---
title: "fileSecurityState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# fileSecurityState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fileHash|[fileHash](../resources/filehash.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|path|String|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileSecurityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileSecurityState",
  "fileHash": {
    "@odata.type": "microsoft.graph.fileHash",
    "hashType": "String",
    "hashValue": "String"
  },
  "name": "String",
  "path": "String",
  "riskScore": "String"
}
```

