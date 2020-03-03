---
title: "emailActivitySummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# emailActivitySummary resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List emailActivitySummaries](../api/emailactivitysummary-list.md)|[emailActivitySummary](../resources/emailActivitySummary.md) collection|List properties and relationships of the [emailActivitySummary](../resources/emailactivitysummary.md) objects.|
|[Get emailActivitySummary](../api/emailactivitysummary-get.md)|[emailActivitySummary](../resources/emailActivitySummary.md)|Read properties and relationships of the [emailActivitySummary](../resources/emailactivitysummary.md) object.|
|[Create emailActivitySummary](../api/emailactivitysummary-create.md)|[emailActivitySummary](../resources/emailActivitySummary.md)|Create a new [emailActivitySummary](../resources/emailactivitysummary.md) object.|
|[Delete emailActivitySummary](../api/emailactivitysummary-delete.md)|None|Deletes a [emailActivitySummary](../resources/emailactivitysummary.md).|
|[Update emailActivitySummary](../api/emailactivitysummary-update.md)|[emailActivitySummary](../resources/emailActivitySummary.md)|Update the properties of a [emailActivitySummary](../resources/emailactivitysummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|read|Int64||
|receive|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|send|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailActivitySummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailActivitySummary",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "send": 1024,
  "receive": 1024,
  "read": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

