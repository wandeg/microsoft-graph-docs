---
title: "onenotePagePreview resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onenotePagePreview resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|links|[onenotePagePreviewLinks](../resources/onenotepagepreviewlinks.md)|**TODO: Add Description**|
|previewText|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onenotePagePreview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenotePagePreview",
  "previewText": "String",
  "links": {
    "@odata.type": "microsoft.graph.onenotePagePreviewLinks",
    "previewImageUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "String"
    }
  }
}
```

