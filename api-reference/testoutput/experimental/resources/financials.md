---
title: "financials resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# financials resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get financials](../api/financials-get.md)|[financials](../resources/financials.md)|Read properties and relationships of the [financials](../resources/financials.md) object.|
|[Update financials](../api/financials-update.md)|[financials](../resources/financials.md)|Update the properties of a [financials](../resources/financials.md) object.|
|[List companies](../api/financials-list-companies.md)|[company](../resources/company.md) collection|Get the companies from the companies navigation property.|
|[Add companies](../api/financials-post-companies.md)|[company](../resources/company.md)|Add companies by posting to the companies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|companies|[company](../resources/company.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.financials",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.financials",
  "id": "String (identifier)"
}
```

