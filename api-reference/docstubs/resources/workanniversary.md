---
title: "WorkAnniversary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# WorkAnniversary resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|location|String||
|logo|String||
|name|String||
|numberOfYears|Int32||
|startedOn|[Date](../resources/date.md)||
|url|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.WorkAnniversary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.WorkAnniversary",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "startedOn": {
    "@odata.type": "microsoft.graph.Date",
    "day": 1024,
    "month": 1024,
    "year": 1024
  },
  "numberOfYears": 1024
}
```

