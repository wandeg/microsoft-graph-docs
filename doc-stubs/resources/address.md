---
title: "Address resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# Address resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|city|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|geographicArea|String|**TODO: Add Description**|
|geographicAreaType|GeographicAreaType|**TODO: Add Description**. Possible values are: `PROVINCE`, `STATE`.|
|line1|String|**TODO: Add Description**|
|line2|String|**TODO: Add Description**|
|line3|String|**TODO: Add Description**|
|line4|String|**TODO: Add Description**|
|postalCode|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.Address"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Address",
  "line1": "String",
  "line2": "String",
  "line3": "String",
  "line4": "String",
  "city": "String",
  "geographicAreaType": "String",
  "geographicArea": "String",
  "postalCode": "String",
  "country": "String"
}
```

