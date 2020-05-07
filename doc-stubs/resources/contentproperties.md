---
title: "contentProperties resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# contentProperties resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|extensions|String collection|**TODO: Add Description**|
|lastModifiedBy|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|metadata|[contentMetadata](../resources/contentmetadata.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

