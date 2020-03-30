---
title: "deviceGeoLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceGeoLocation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|altitude|Double||
|heading|Double||
|horizontalAccuracy|Double||
|lastCollectedDateTime|DateTimeOffset||
|lastCollectedDateTimeUtc|DateTimeOffset||
|latitude|Double||
|longitude|Double||
|speed|Double||
|verticalAccuracy|Double||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
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

