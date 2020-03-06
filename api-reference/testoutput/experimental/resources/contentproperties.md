---
title: "contentProperties resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# contentProperties resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|extensions|String collection||
|lastModifiedBy|String||
|lastModifiedDateTime|DateTimeOffset||
|metadata|[contentMetadata](../resources/contentmetadata.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.contentProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentProperties",
  "extensions": [
    "String"
  ],
  "metadata": {
    "@odata.type": "microsoft.graph.contentMetadata"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": "String"
}
```

