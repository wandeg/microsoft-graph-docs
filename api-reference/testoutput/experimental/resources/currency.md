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
|[List currencies](../api/currency-list.md)|[currency](../resources/currency.md) collection|List properties and relationships of the [currency](../resources/currency.md) objects.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|
|[Create currency](../api/currency-create.md)|[currency](../resources/currency.md)|Create a new [currency](../resources/currency.md) object.|
|[Delete currency](../api/currency-delete.md)|None|Deletes a [currency](../resources/currency.md).|
|[Update currency](../api/currency-update.md)|[currency](../resources/currency.md)|Update the properties of a [currency](../resources/currency.md) object.|

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

## JSON Representation
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

