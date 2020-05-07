---
title: "SalesNavigatorInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# SalesNavigatorInfo resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contractChooserUrl|String|**TODO: Add Description**|
|contractName|String|**TODO: Add Description**|
|insights|[SalesNavigatorInsight](../resources/salesnavigatorinsight.md) collection|**TODO: Add Description**|
|profileUrl|String|**TODO: Add Description**|
|savedAccount|[LinkedInOrganization](../resources/linkedinorganization.md)|**TODO: Add Description**|
|savedLead|Boolean|**TODO: Add Description**|
|teamlinkInfo|[SalesNavigatorTeamlinkInfo](../resources/salesnavigatorteamlinkinfo.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SalesNavigatorInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SalesNavigatorInfo",
  "profileUrl": "String",
  "teamlinkInfo": {
    "@odata.type": "microsoft.graph.SalesNavigatorTeamlinkInfo"
  },
  "insights": [
    {
      "@odata.type": "microsoft.graph.SalesNavigatorInsight"
    }
  ],
  "savedLead": "Boolean",
  "savedAccount": {
    "@odata.type": "microsoft.graph.LinkedInOrganization"
  },
  "contractName": "String",
  "contractChooserUrl": "String"
}
```

