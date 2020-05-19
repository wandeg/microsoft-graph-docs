---
title: "automaticRepliesMailTips resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "scheduledStartTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "scheduledEndTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

