---
title: "MeetNewHire resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# MeetNewHire resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|hiredOn|[Date](../resources/date.md)||
|location|String||
|logo|String||
|name|String||
|url|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.MeetNewHire"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.MeetNewHire",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "hiredOn": {
    "@odata.type": "microsoft.graph.Date",
    "day": 1024,
    "month": 1024,
    "year": 1024
  }
}
```

