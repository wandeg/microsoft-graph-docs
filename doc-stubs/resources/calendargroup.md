---
title: "calendarGroup resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# calendarGroup resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List calendars](../api/calendargroup-list-calendars.md)|[calendar](../resources/calendar.md) collection|Get the calendars from the calendars navigation property.|
|[Create calendars](../api/calendargroup-post-calendars.md)|[calendar](../resources/calendar.md)|Create a new calendars object.|
|[Delete calendars](../api/calendargroup-delete-calendars.md)|None|Delete a [calendar](../resources/calendar.md) object.|
|[Update calendars](../api/calendargroup-update-calendars.md)|[calendar](../resources/calendar.md)|Update the properties of a calendars object.|
|[Get calendar](../api/calendar-get.md)|[calendar](../resources/calendar.md)|Read the properties and relationships of a [calendar](../resources/calendar.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeKey|String|**TODO: Add Description**|
|classId|Guid|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|calendars|[calendar](../resources/calendar.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "id": "String (identifier)",
  "name": "String",
  "classId": "Guid",
  "changeKey": "String"
}
```

