---
title: "siteActivitySummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# siteActivitySummary resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List siteActivitySummaries](../api/siteactivitysummary-list.md)|[siteActivitySummary](../resources/siteActivitySummary.md) collection|List properties and relationships of the [siteActivitySummary](../resources/siteactivitysummary.md) objects.|
|[Get siteActivitySummary](../api/siteactivitysummary-get.md)|[siteActivitySummary](../resources/siteActivitySummary.md)|Read properties and relationships of the [siteActivitySummary](../resources/siteactivitysummary.md) object.|
|[Create siteActivitySummary](../api/siteactivitysummary-create.md)|[siteActivitySummary](../resources/siteActivitySummary.md)|Create a new [siteActivitySummary](../resources/siteactivitysummary.md) object.|
|[Delete siteActivitySummary](../api/siteactivitysummary-delete.md)|None|Deletes a [siteActivitySummary](../resources/siteactivitysummary.md).|
|[Update siteActivitySummary](../api/siteactivitysummary-update.md)|[siteActivitySummary](../resources/siteActivitySummary.md)|Update the properties of a [siteActivitySummary](../resources/siteactivitysummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|sharedExternally|Int64||
|sharedInternally|Int64||
|synced|Int64||
|viewedOrEdited|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.siteActivitySummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.siteActivitySummary",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "viewedOrEdited": 1024,
  "synced": 1024,
  "sharedInternally": 1024,
  "sharedExternally": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

