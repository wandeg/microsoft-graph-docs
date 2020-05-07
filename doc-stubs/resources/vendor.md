---
title: "vendor resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# vendor resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List picture](../api/vendor-list-picture.md)|[picture](../resources/picture.md) collection|Get the pictures from the picture navigation property.|
|[Create picture](../api/vendor-post-picture.md)|[picture](../resources/picture.md)|Create a new picture object.|
|[Delete picture](../api/vendor-delete-picture.md)|None|Delete a [picture](../resources/picture.md) object.|
|[Update picture](../api/vendor-update-picture.md)|[picture](../resources/picture.md)|Update the properties of a picture object.|
|[Get picture](../api/picture-get.md)|[picture](../resources/picture.md)|Read the properties and relationships of a [picture](../resources/picture.md) object.|
|[List currency](../api/vendor-list-currency.md)|[currency](../resources/currency.md) collection|Get the currencies from the currency navigation property.|
|[Create currency](../api/vendor-post-currency.md)|[currency](../resources/currency.md)|Create a new currency object.|
|[Delete currency](../api/vendor-delete-currency.md)|None|Delete a [currency](../resources/currency.md) object.|
|[Update currency](../api/vendor-update-currency.md)|[currency](../resources/currency.md)|Update the properties of a currency object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read the properties and relationships of a [currency](../resources/currency.md) object.|
|[List paymentTerm](../api/vendor-list-paymentterm.md)|[paymentTerm](../resources/paymentterm.md) collection|Get the paymentTerms from the paymentTerm navigation property.|
|[Create paymentTerm](../api/vendor-post-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Create a new paymentTerm object.|
|[Delete paymentTerm](../api/vendor-delete-paymentterm.md)|None|Delete a [paymentTerm](../resources/paymentterm.md) object.|
|[Update paymentTerm](../api/vendor-update-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Update the properties of a paymentTerm object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read the properties and relationships of a [paymentTerm](../resources/paymentterm.md) object.|
|[List paymentMethod](../api/vendor-list-paymentmethod.md)|[paymentMethod](../resources/paymentmethod.md) collection|Get the paymentMethods from the paymentMethod navigation property.|
|[Create paymentMethod](../api/vendor-post-paymentmethod.md)|[paymentMethod](../resources/paymentmethod.md)|Create a new paymentMethod object.|
|[Delete paymentMethod](../api/vendor-delete-paymentmethod.md)|None|Delete a [paymentMethod](../resources/paymentmethod.md) object.|
|[Update paymentMethod](../api/vendor-update-paymentmethod.md)|[paymentMethod](../resources/paymentmethod.md)|Update the properties of a paymentMethod object.|
|[Get paymentMethod](../api/paymentmethod-get.md)|[paymentMethod](../resources/paymentmethod.md)|Read the properties and relationships of a [paymentMethod](../resources/paymentmethod.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|balance|Decimal|**TODO: Add Description**|
|blocked|String|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|number|String|**TODO: Add Description**|
|paymentMethodId|Guid|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|taxLiable|Boolean|**TODO: Add Description**|
|taxRegistrationNumber|String|**TODO: Add Description**|
|website|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)|**TODO: Add Description**|
|paymentMethod|[paymentMethod](../resources/paymentmethod.md)|**TODO: Add Description**|
|paymentTerm|[paymentTerm](../resources/paymentterm.md)|**TODO: Add Description**|
|picture|[picture](../resources/picture.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vendor",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vendor",
  "id": "String (identifier)",
  "number": "String",
  "displayName": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "email": "String",
  "website": "String",
  "taxRegistrationNumber": "String",
  "currencyId": "Guid",
  "currencyCode": "String",
  "paymentTermsId": "Guid",
  "paymentMethodId": "Guid",
  "taxLiable": "Boolean",
  "blocked": "String",
  "balance": "Decimal",
  "lastModifiedDateTime": "String (timestamp)"
}
```

