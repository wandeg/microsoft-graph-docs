---
title: "requiredResourceAccess resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# requiredResourceAccess resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|resourceAccess|[resourceAccess](../resources/resourceaccess.md) collection|**TODO: Add Description**|
|resourceAppId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requiredResourceAccess",
  "resourceAppId": "String",
  "resourceAccess": [
    {
      "@odata.type": "microsoft.graph.resourceAccess"
    }
  ]
}
```

