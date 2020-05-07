---
title: "visualInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# visualInfo resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attribution|[imageInfo](../resources/imageinfo.md)|**TODO: Add Description**|
|backgroundColor|String|**TODO: Add Description**|
|content|[Json](../resources/json.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayText|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.visualInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.visualInfo",
  "attribution": {
    "@odata.type": "microsoft.graph.imageInfo"
  },
  "backgroundColor": "String",
  "description": "String",
  "displayText": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

