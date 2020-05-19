---
title: "WorkAnniversary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# WorkAnniversary resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|location|String|**TODO: Add Description**|
|logo|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|numberOfYears|Int32|**TODO: Add Description**|
|startedOn|[Date](../resources/date.md)|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.WorkAnniversary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.WorkAnniversary",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "startedOn": {
    "@odata.type": "microsoft.graph.Date"
  },
  "numberOfYears": "Integer"
}
```

