---
title: "SalesNavigatorTeamlinkInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# SalesNavigatorTeamlinkInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|countOfTotalTeamlinkConnections|Int32||
|teamlinkSearchUrl|String||
|topTeamlinks|[SalesNavigatorPersonInfo](../resources/salesnavigatorpersoninfo.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SalesNavigatorTeamlinkInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SalesNavigatorTeamlinkInfo",
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
}
```

