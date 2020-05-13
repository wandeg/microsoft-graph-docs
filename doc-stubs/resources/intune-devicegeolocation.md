---
title: "deviceGeoLocation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceGeoLocation resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|altitude|Double|**TODO: Add Description**|
|heading|Double|**TODO: Add Description**|
|horizontalAccuracy|Double|**TODO: Add Description**|
|lastCollectedDateTime|DateTimeOffset|**TODO: Add Description**|
|latitude|Double|**TODO: Add Description**|
|longitude|Double|**TODO: Add Description**|
|speed|Double|**TODO: Add Description**|
|verticalAccuracy|Double|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "Double",
  "latitude": "Double",
  "altitude": "Double",
  "horizontalAccuracy": "Double",
  "verticalAccuracy": "Double",
  "heading": "Double",
  "speed": "Double"
}
```

