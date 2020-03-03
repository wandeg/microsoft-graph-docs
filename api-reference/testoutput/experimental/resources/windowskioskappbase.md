---
title: "windowsKioskAppBase resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsKioskAppBase resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appType|Enumeration|The app type. Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean|Allow the app to be auto-launched in multi-app kiosk mode|
|name|String|Represents the friendly name of an app|
|startLayoutTileSize|Enumeration|The app tile size for the start layout. Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

## Relationships
None

## JSON Representation
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

