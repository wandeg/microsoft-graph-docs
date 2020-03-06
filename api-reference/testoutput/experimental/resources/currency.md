---
title: "currency resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# currency resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|
|[Update currency](../api/currency-update.md)|[currency](../resources/currency.md)|Update the properties of a [currency](../resources/currency.md) object.|
|[List currencies](../api/company-list-currencies.md)|[currency](../resources/currency.md) collection|Get the currencies from the currencies navigation property.|
|[Add currencies](../api/company-post-currencies.md)|[currency](../resources/currency.md)|Add currencies by posting to the currencies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|amountDecimalPlaces|String||
|amountRoundingPrecision|Decimal||
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|symbol|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.currency",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.currency",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "symbol": "String",
  "amountDecimalPlaces": "String",
  "amountRoundingPrecision": "4.2",
  "lastModifiedDateTime": "String (timestamp)"
}
```

