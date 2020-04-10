---
title: "windowsKioskUWPApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsKioskUWPApp resource type


Namespace: microsoft.graph




Inherits from [windowsKioskAppBase](../resources/windowskioskappbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String||
|appType|Enumeration| Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|appUserModelId|String||
|autoLaunch|Boolean| Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|containedAppId|String||
|name|String| Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|startLayoutTileSize|Enumeration| Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```

