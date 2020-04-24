---
title: "windowsKioskAppBase resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsKioskAppBase resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appType|windowsKioskAppType|The app type. Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean|Allow the app to be auto-launched in multi-app kiosk mode|
|name|String|Represents the friendly name of an app|
|startLayoutTileSize|windowsAppStartLayoutTileSize|The app tile size for the start layout. Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

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

