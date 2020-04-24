---
title: "windowsKioskMultipleApps resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsKioskMultipleApps resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [windowsKioskAppConfiguration](../resources/windowskioskappconfiguration.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowAccessToDownloadsFolder|Boolean|This setting allows access to Downloads folder in file explorer.|
|apps|[windowsKioskAppBase](../resources/windowskioskappbase.md) collection|These are the only Windows Store Apps that will be available to launch from the Start menu. This collection can contain a maximum of 128 elements.|
|disallowDesktopApps|Boolean|This setting indicates that desktop apps are allowed. Default to true.|
|showTaskBar|Boolean|This setting allows the admin to specify whether the Task Bar is shown or not.|
|startMenuLayoutXml|Binary|Allows admins to override the default Start layout and prevents the user from changing it. The layout is modified by specifying an XML file based on a layout modification schema. XML needs to be in Binary format.|

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

