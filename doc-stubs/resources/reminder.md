---
title: "reminder resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# reminder resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeKey|String|**TODO: Add Description**|
|eventEndTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|eventId|String|**TODO: Add Description**|
|eventLocation|[location](../resources/location.md)|**TODO: Add Description**|
|eventStartTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|eventSubject|String|**TODO: Add Description**|
|eventWebLink|String|**TODO: Add Description**|
|reminderFireTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.reminder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reminder",
  "eventId": "String",
  "eventStartTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "eventEndTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "changeKey": "String",
  "eventSubject": "String",
  "eventLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "eventWebLink": "String",
  "reminderFireTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

