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
|appType|Enumeration|The app type Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean|Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|desktopApplicationId|String|Define the DesktopApplicationID of the app|
|desktopApplicationLinkPath|String|Define the DesktopApplicationLinkPath of the app|
|name|String|Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|path|String|Define the path of a desktop app|
|startLayoutTileSize|Enumeration|The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

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

