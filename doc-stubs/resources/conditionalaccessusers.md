---
title: "conditionalAccessUsers resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# conditionalAccessUsers resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeGroups|String collection|**TODO: Add Description**|
|excludeRoles|String collection|**TODO: Add Description**|
|excludeUsers|String collection|**TODO: Add Description**|
|includeGroups|String collection|**TODO: Add Description**|
|includeRoles|String collection|**TODO: Add Description**|
|includeUsers|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessUsers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessUsers",
  "includeUsers": [
    "String"
  ],
  "excludeUsers": [
    "String"
  ],
  "includeGroups": [
    "String"
  ],
  "excludeGroups": [
    "String"
  ],
  "includeRoles": [
    "String"
  ],
  "excludeRoles": [
    "String"
  ]
}
```

