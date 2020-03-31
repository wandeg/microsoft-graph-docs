---
title: "provisionedIdentity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# provisionedIdentity resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|details|[detailsInfo](../resources/detailsinfo.md)||
|displayName|String||
|id|String||
|identityType|String||

## Relationships
None

## JSON representation
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

