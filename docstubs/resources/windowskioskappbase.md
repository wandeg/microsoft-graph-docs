---
title: "windowsKioskAppBase resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsKioskAppBase resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appType|Enumeration| Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean||
|name|String||
|startLayoutTileSize|Enumeration| Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```

