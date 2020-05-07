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


Inherits from [windowsKioskAppConfiguration](../resources/windowskioskappconfiguration.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowAccessToDownloadsFolder|Boolean|**TODO: Add Description**|
|apps|[windowsKioskAppBase](../resources/windowskioskappbase.md) collection|**TODO: Add Description**|
|disallowDesktopApps|Boolean|**TODO: Add Description**|
|showTaskBar|Boolean|**TODO: Add Description**|
|startMenuLayoutXml|Binary|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.windowsKioskUWPApp"
    }
  ],
  "showTaskBar": "Boolean",
  "allowAccessToDownloadsFolder": "Boolean",
  "disallowDesktopApps": "Boolean",
  "startMenuLayoutXml": "Binary"
}
```

