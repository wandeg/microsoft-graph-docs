---
title: "onlineMeetingInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onlineMeetingInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|conferenceId|String||
|joinUrl|String||
|phones|[phone](../resources/phone.md) collection||
|quickDial|String||
|tollFreeNumbers|String collection||
|tollNumber|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onlineMeetingInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onlineMeetingInfo",
  "joinUrl": "String",
  "conferenceId": "String",
  "tollNumber": "String",
  "tollFreeNumbers": [
    "String"
  ],
  "quickDial": "String",
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone",
      "type": "String",
      "number": "String",
      "region": "String",
      "language": "String"
    }
  ]
}
```

