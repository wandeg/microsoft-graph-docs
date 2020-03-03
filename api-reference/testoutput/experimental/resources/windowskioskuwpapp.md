---
title: "windowsKioskUWPApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsKioskUWPApp resource type




Inherits from [windowsKioskAppBase](../resources/windowsKioskAppBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String|This references an Intune App that will be target to the same assignments as Kiosk configuration|
|appType|Enumeration|The app type Inherited from [windowsKioskAppBase](../resources/windowsKioskAppBase.md). Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|appUserModelId|String|This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode|
|autoLaunch|Boolean|Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/windowsKioskAppBase.md)|
|containedAppId|String|This references an contained App from an Intune App|
|name|String|Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/windowsKioskAppBase.md)|
|startLayoutTileSize|Enumeration|The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/windowsKioskAppBase.md). Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

## Relationships
None

## JSON Representation
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

