---
title: "automaticRepliesMailTips resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# automaticRepliesMailTips resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|message|String|**TODO: Add Description**|
|messageLanguage|[localeInfo](../resources/localeinfo.md)|**TODO: Add Description**|
|scheduledEndTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|scheduledStartTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

