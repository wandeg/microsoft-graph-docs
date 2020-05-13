---
title: "LIOrganization resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIOrganization resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|industries|[LIIndustry](../resources/liindustry.md) collection|**TODO: Add Description**|
|locations|[LIOrganizationLocationInfo](../resources/liorganizationlocationinfo.md) collection|**TODO: Add Description**|
|logoV2|String|**TODO: Add Description**|
|name|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|website|[MultiLocaleUrl](../resources/multilocaleurl.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIOrganization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIOrganization",
  "id": "String (identifier)",
  "name": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "logoV2": "String",
  "website": {
    "@odata.type": "microsoft.graph.MultiLocaleUrl"
  },
  "locations": [
    {
      "@odata.type": "microsoft.graph.LIOrganizationLocationInfo"
    }
  ],
  "industries": [
    {
      "@odata.type": "microsoft.graph.LIIndustry"
    }
  ]
}
```

