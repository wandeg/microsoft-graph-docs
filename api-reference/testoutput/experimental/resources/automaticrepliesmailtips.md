---
title: "automaticRepliesMailTips resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# automaticRepliesMailTips resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|message|String||
|messageLanguage|[localeInfo](../resources/localeInfo.md)||
|scheduledEndTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|scheduledStartTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.automaticRepliesMailTips",
  "message": "String",
  "messageLanguage": {
    "@odata.type": "microsoft.graph.localeInfo",
    "locale": "String",
    "displayName": "String"
  },
  "scheduledStartTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "scheduledEndTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

