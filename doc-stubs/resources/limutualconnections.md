---
title: "LIMutualConnections resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIMutualConnections resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|mutualConnections|[LIMemberDetails](../resources/limemberdetails.md) collection|**TODO: Add Description**|
|mutualConnectionsPage|String|**TODO: Add Description**|
|totalCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMutualConnections"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMutualConnections",
  "mutualConnections": [
    {
      "@odata.type": "microsoft.graph.LIMemberDetails"
    }
  ],
  "totalCount": "Integer",
  "mutualConnectionsPage": "String"
}
```

