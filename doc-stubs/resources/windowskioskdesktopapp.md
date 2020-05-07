---
title: "windowsKioskDesktopApp resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsKioskDesktopApp resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [windowsKioskAppBase](../resources/windowskioskappbase.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appType|windowsKioskAppType|**TODO: Add Description** Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean|**TODO: Add Description** Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|desktopApplicationId|String|**TODO: Add Description**|
|desktopApplicationLinkPath|String|**TODO: Add Description**|
|name|String|**TODO: Add Description** Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md)|
|path|String|**TODO: Add Description**|
|startLayoutTileSize|windowsAppStartLayoutTileSize|**TODO: Add Description** Inherited from [windowsKioskAppBase](../resources/windowskioskappbase.md). Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "autoLaunch": "Boolean",
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```

