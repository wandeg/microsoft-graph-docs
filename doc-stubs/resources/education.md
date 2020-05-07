---
title: "Education resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# Education resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|degreeName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|fieldOfStudy|String|**TODO: Add Description**|
|location|String|**TODO: Add Description**|
|logo|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|startEndDate|[DateRange](../resources/daterange.md)|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.Education"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Education",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "degreeName": "String",
  "startEndDate": {
    "@odata.type": "microsoft.graph.DateRange"
  },
  "fieldOfStudy": "String",
  "description": "String"
}
```

