---
title: "windowsKioskSingleUWPApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsKioskSingleUWPApp resource type


Namespace: microsoft.graph




Inherits from [windowsKioskAppConfiguration](../resources/windowskioskappconfiguration.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|uwpApp|[windowsKioskUWPApp](../resources/windowskioskuwpapp.md)|This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```

