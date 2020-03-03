---
title: "deviceKey resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceKey resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|Guid||
|keyMaterial|Binary||
|keyType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceKey",
  "keyType": "String",
  "keyMaterial": "binary",
  "deviceId": "Guid"
}
```

