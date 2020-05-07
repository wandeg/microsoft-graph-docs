---
title: "positionDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# positionDetail resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|company|[companyDetail](../resources/companydetail.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|endMonthYear|Date|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|role|String|**TODO: Add Description**|
|startMonthYear|Date|**TODO: Add Description**|
|summary|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.positionDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.positionDetail",
  "company": {
    "@odata.type": "microsoft.graph.companyDetail"
  },
  "description": "String",
  "endMonthYear": "Date",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "Date",
  "summary": "String"
}
```

