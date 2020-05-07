---
title: "bookingCurrency resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingCurrency resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List bookingCurrencies](../api/bookingcurrency-list.md)|[bookingCurrency](../resources/bookingcurrency.md) collection|Get a list of the [bookingCurrency](../resources/bookingcurrency.md) objects and their properties.|
|[Get bookingCurrency](../api/bookingcurrency-get.md)|[bookingCurrency](../resources/bookingcurrency.md)|Read the properties and relationships of a [bookingCurrency](../resources/bookingcurrency.md) object.|
|[Create bookingCurrency](../api/bookingcurrency-post-bookingcurrencies.md)|[bookingCurrency](../resources/bookingcurrency.md)|Create a new [bookingCurrency](../resources/bookingcurrency.md) object.|
|[Delete bookingCurrency](../api/bookingcurrency-delete.md)|None|Deletes a [bookingCurrency](../resources/bookingcurrency.md) object.|
|[Update bookingCurrency](../api/bookingcurrency-update.md)|[bookingCurrency](../resources/bookingcurrency.md)|Update the properties of a [bookingCurrency](../resources/bookingcurrency.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|symbol|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCurrency",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCurrency",
  "id": "String (identifier)",
  "symbol": "String"
}
```

