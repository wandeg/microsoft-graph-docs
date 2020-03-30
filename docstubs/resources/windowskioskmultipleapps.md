---
title: "windowsKioskMultipleApps resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsKioskMultipleApps resource type


Namespace: microsoft.graph




Inherits from [windowsKioskAppConfiguration](../resources/windowskioskappconfiguration.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowAccessToDownloadsFolder|Boolean||
|apps|[windowsKioskAppBase](../resources/windowskioskappbase.md) collection||
|disallowDesktopApps|Boolean||
|showTaskBar|Boolean||
|startMenuLayoutXml|Binary||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appType": "String",
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```

