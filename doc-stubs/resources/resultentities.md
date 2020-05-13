---
title: "ResultEntities resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# ResultEntities resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|lIFieldOfStudyArray|[LIFieldOfStudyArray](../resources/lifieldofstudyarray.md)|**TODO: Add Description**|
|lILocationArray|[LILocationArray](../resources/lilocationarray.md)|**TODO: Add Description**|
|lIMemberArray|[LIMemberArray](../resources/limemberarray.md)|**TODO: Add Description**|
|lIOrganizationArray|[LIOrganizationArray](../resources/liorganizationarray.md)|**TODO: Add Description**|
|lISkillArray|[LISkillArray](../resources/liskillarray.md)|**TODO: Add Description**|
|lITitleArray|[LITitleArray](../resources/lititlearray.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ResultEntities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ResultEntities",
  "lIMemberArray": {
    "@odata.type": "microsoft.graph.LIMemberArray"
  },
  "lIFieldOfStudyArray": {
    "@odata.type": "microsoft.graph.LIFieldOfStudyArray"
  },
  "lILocationArray": {
    "@odata.type": "microsoft.graph.LILocationArray"
  },
  "lIOrganizationArray": {
    "@odata.type": "microsoft.graph.LIOrganizationArray"
  },
  "lISkillArray": {
    "@odata.type": "microsoft.graph.LISkillArray"
  },
  "lITitleArray": {
    "@odata.type": "microsoft.graph.LITitleArray"
  }
}
```

