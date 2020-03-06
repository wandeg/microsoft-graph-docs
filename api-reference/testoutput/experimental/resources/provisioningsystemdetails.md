---
title: "provisioningSystemDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# provisioningSystemDetails resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|details|[detailsInfo](../resources/detailsinfo.md)||
|displayName|String||
|id|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisioningSystemDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisioningSystemDetails",
  "id": "String (identifier)",
  "displayName": "String",
  "details": {
    "@odata.type": "microsoft.graph.detailsInfo"
  }
}
```

