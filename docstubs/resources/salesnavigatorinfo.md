---
title: "SalesNavigatorInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# SalesNavigatorInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|contractChooserUrl|String||
|contractName|String||
|insights|[SalesNavigatorInsight](../resources/salesnavigatorinsight.md) collection||
|profileUrl|String||
|savedAccount|[LinkedInOrganization](../resources/linkedinorganization.md)||
|savedLead|Boolean||
|teamlinkInfo|[SalesNavigatorTeamlinkInfo](../resources/salesnavigatorteamlinkinfo.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.SalesNavigatorTeamlinkInfo",
    "countOfTotalTeamlinkConnections": 1024,
    "teamlinkSearchUrl": "String",
    "topTeamlinks": [
      {
        "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo",
        "firstName": "String",
        "lastName": "String",
        "url": "String",
        "photoUrl": "String"
      }
    ]
  },
  "insights": [
    {
      "@odata.type": "microsoft.graph.SalesNavigatorInsight",
      "createdAt": 1024,
      "insightType": "String",
      "title": "String",
      "detail": "String",
      "insightUrl": "String",
      "person": {
        "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo"
      }
    }
  ],
  "savedLead": true,
  "savedAccount": {
    "@odata.type": "microsoft.graph.LinkedInOrganization",
    "name": "String",
    "logo": "String",
    "location": "String"
  },
  "contractName": "String",
  "contractChooserUrl": "String"
}
```

