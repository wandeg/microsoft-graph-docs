---
title: "edgeSearchEngine resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# edgeSearchEngine resource type




Inherits from [edgeSearchEngineBase](../resources/edgeSearchEngineBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|edgeSearchEngineType|Enumeration|Allows IT admins to set a predefined default search engine for MDM-Controlled devices. Possible values are: `default`, `bing`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```

