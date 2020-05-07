---
title: "LIMemberEducation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIMemberEducation resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activities|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|degreeName|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|endMonthYear|[Date](../resources/date.md)|**TODO: Add Description**|
|fieldsOfStudy|[LIMemberFieldOfStudy](../resources/limemberfieldofstudy.md) collection|**TODO: Add Description**|
|fieldsOfStudyV2|[LIFieldOfStudy](../resources/lifieldofstudy.md) collection|**TODO: Add Description**|
|notes|[MultiLocaleRichText](../resources/multilocalerichtext.md)|**TODO: Add Description**|
|school|[LIOrganization](../resources/liorganization.md)|**TODO: Add Description**|
|startMonthYear|[Date](../resources/date.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberEducation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberEducation",
  "degreeName": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "activities": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "startMonthYear": {
    "@odata.type": "microsoft.graph.Date"
  },
  "endMonthYear": {
    "@odata.type": "microsoft.graph.Date"
  },
  "notes": {
    "@odata.type": "microsoft.graph.MultiLocaleRichText"
  },
  "school": {
    "@odata.type": "microsoft.graph.LIOrganization"
  },
  "fieldsOfStudy": [
    {
      "@odata.type": "microsoft.graph.LIMemberFieldOfStudy"
    }
  ],
  "fieldsOfStudyV2": [
    {
      "@odata.type": "microsoft.graph.LIFieldOfStudy"
    }
  ]
}
```

