---
title: "vendor resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# vendor resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get vendor](../api/vendor-get.md)|[vendor](../resources/vendor.md)|Read properties and relationships of the [vendor](../resources/vendor.md) object.|
|[Update vendor](../api/vendor-update.md)|[vendor](../resources/vendor.md)|Update the properties of a [vendor](../resources/vendor.md) object.|
|[List picture](../api/vendor-list-picture.md)|[picture](../resources/picture.md) collection|Get the pictures from the picture navigation property.|
|[Add picture](../api/vendor-post-picture.md)|[picture](../resources/picture.md)|Add picture by posting to the picture collection.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.|
|[Get paymentMethod](../api/paymentmethod-get.md)|[paymentMethod](../resources/paymentmethod.md)|Read properties and relationships of the [paymentMethod](../resources/paymentmethod.md) object.|
|[List vendors](../api/company-list-vendors.md)|[vendor](../resources/vendor.md) collection|Get the vendors from the vendors navigation property.|
|[Add vendors](../api/company-post-vendors.md)|[vendor](../resources/vendor.md)|Add vendors by posting to the vendors collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[postalAddressType](../resources/postaladdresstype.md)||
|balance|Decimal||
|blocked|String||
|currencyCode|String||
|currencyId|Guid||
|displayName|String||
|email|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|number|String||
|paymentMethodId|Guid||
|paymentTermsId|Guid||
|phoneNumber|String||
|taxLiable|Boolean||
|taxRegistrationNumber|String||
|website|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)||
|paymentMethod|[paymentMethod](../resources/paymentmethod.md)||
|paymentTerm|[paymentTerm](../resources/paymentterm.md)||
|picture|[picture](../resources/picture.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.postalAddressType",
    "street": "String",
    "city": "String",
    "state": "String",
    "countryLetterCode": "String",
    "postalCode": "String"
  },
  "phoneNumber": "String",
  "email": "String",
  "website": "String",
  "taxRegistrationNumber": "String",
  "currencyId": "Guid",
  "currencyCode": "String",
  "paymentTermsId": "Guid",
  "paymentMethodId": "Guid",
  "taxLiable": true,
  "blocked": "String",
  "balance": "4.2",
  "lastModifiedDateTime": "String (timestamp)"
}
```

