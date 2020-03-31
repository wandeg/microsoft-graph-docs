---
title: "windowsKioskDesktopApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsKioskDesktopApp resource type


Namespace: microsoft.graph




Inherits from [windowsKioskAppBase](../resources/windowskioskappbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appType|Enumeration| Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean| Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|desktopApplicationId|String||
|desktopApplicationLinkPath|String||
|name|String| Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|path|String||
|startLayoutTileSize|Enumeration| Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```

