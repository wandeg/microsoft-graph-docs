---
title: "file resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# file resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|hashes|[hashes](../resources/hashes.md)|**TODO: Add Description**|
|mimeType|String|**TODO: Add Description**|
|processingMetadata|Boolean|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.file"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.file",
  "hashes": {
    "@odata.type": "microsoft.graph.hashes",
    "crc32Hash": "String",
    "quickXorHash": "String",
    "sha1Hash": "String",
    "sha256Hash": "String"
  },
  "mimeType": "String",
  "processingMetadata": true
}
```

