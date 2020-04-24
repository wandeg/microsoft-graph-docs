---
title: "windowsKioskUWPApp resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsKioskUWPApp resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [windowsKioskAppBase](../resources/windowskioskappbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String|This references an Intune App that will be target to the same assignments as Kiosk configuration|
|appType|windowsKioskAppType|The app type Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|appUserModelId|String|This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode|
|autoLaunch|Boolean|Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|containedAppId|String|This references an contained App from an Intune App|
|name|String|Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|startLayoutTileSize|windowsAppStartLayoutTileSize|The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

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

