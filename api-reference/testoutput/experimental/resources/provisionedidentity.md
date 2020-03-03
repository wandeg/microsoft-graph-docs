---
title: "provisionedIdentity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# provisionedIdentity resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|details|[detailsInfo](../resources/detailsInfo.md)||
|displayName|String||
|id|String||
|identityType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisionedIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisionedIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "identityType": "String",
  "details": {
    "@odata.type": "microsoft.graph.detailsInfo"
  }
}
```

