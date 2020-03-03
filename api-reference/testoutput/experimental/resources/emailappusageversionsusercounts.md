---
title: "emailAppUsageVersionsUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# emailAppUsageVersionsUserCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List emailAppUsageVersionsUserCountses](../api/emailappusageversionsusercounts-list.md)|[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) collection|List properties and relationships of the [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) objects.|
|[Get emailAppUsageVersionsUserCounts](../api/emailappusageversionsusercounts-get.md)|[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)|Read properties and relationships of the [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object.|
|[Create emailAppUsageVersionsUserCounts](../api/emailappusageversionsusercounts-create.md)|[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)|Create a new [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object.|
|[Delete emailAppUsageVersionsUserCounts](../api/emailappusageversionsusercounts-delete.md)|None|Deletes a [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md).|
|[Update emailAppUsageVersionsUserCounts](../api/emailappusageversionsusercounts-update.md)|[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)|Update the properties of a [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|outlook2007|Int64||
|outlook2010|Int64||
|outlook2013|Int64||
|outlook2016|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|undetermined|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAppUsageVersionsUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "outlook2016": 1024,
  "outlook2013": 1024,
  "outlook2010": 1024,
  "outlook2007": 1024,
  "undetermined": 1024,
  "reportPeriod": "String"
}
```

