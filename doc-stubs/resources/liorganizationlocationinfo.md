---
title: "LIOrganizationLocationInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIOrganizationLocationInfo resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[Address](../resources/address.md)|**TODO: Add Description**|
|locationType|LILocationType|**TODO: Add Description**. Possible values are: `HEADQUARTERS`, `OTHER`.|
|standardizedLocation|[LILocation](../resources/lilocation.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIOrganizationLocationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIOrganizationLocationInfo",
  "address": {
    "@odata.type": "microsoft.graph.Address"
  },
  "locationType": "String",
  "standardizedLocation": {
    "@odata.type": "microsoft.graph.LILocation"
  }
}
```

