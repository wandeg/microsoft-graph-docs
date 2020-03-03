---
title: "yammerActivitySummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# yammerActivitySummary resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List yammerActivitySummaries](../api/yammeractivitysummary-list.md)|[yammerActivitySummary](../resources/yammerActivitySummary.md) collection|List properties and relationships of the [yammerActivitySummary](../resources/yammeractivitysummary.md) objects.|
|[Get yammerActivitySummary](../api/yammeractivitysummary-get.md)|[yammerActivitySummary](../resources/yammerActivitySummary.md)|Read properties and relationships of the [yammerActivitySummary](../resources/yammeractivitysummary.md) object.|
|[Create yammerActivitySummary](../api/yammeractivitysummary-create.md)|[yammerActivitySummary](../resources/yammerActivitySummary.md)|Create a new [yammerActivitySummary](../resources/yammeractivitysummary.md) object.|
|[Delete yammerActivitySummary](../api/yammeractivitysummary-delete.md)|None|Deletes a [yammerActivitySummary](../resources/yammeractivitysummary.md).|
|[Update yammerActivitySummary](../api/yammeractivitysummary-update.md)|[yammerActivitySummary](../resources/yammerActivitySummary.md)|Update the properties of a [yammerActivitySummary](../resources/yammeractivitysummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|liked|Int64||
|posted|Int64||
|read|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.yammerActivitySummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.yammerActivitySummary",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "liked": 1024,
  "posted": 1024,
  "read": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

