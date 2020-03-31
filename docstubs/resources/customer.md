---
title: "customer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# customer resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read properties and relationships of the [customer](../resources/customer.md) object.|
|[Update customer](../api/customer-update.md)|[customer](../resources/customer.md)|Update the properties of a [customer](../resources/customer.md) object.|
|[List picture](../api/customer-list-picture.md)|[picture](../resources/picture.md) collection|Get the pictures from the picture navigation property.|
|[Add picture](../api/customer-post-picture.md)|[picture](../resources/picture.md)|Add picture by posting to the picture collection.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.|
|[Get shipmentMethod](../api/shipmentmethod-get.md)|[shipmentMethod](../resources/shipmentmethod.md)|Read properties and relationships of the [shipmentMethod](../resources/shipmentmethod.md) object.|
|[Get paymentMethod](../api/paymentmethod-get.md)|[paymentMethod](../resources/paymentmethod.md)|Read properties and relationships of the [paymentMethod](../resources/paymentmethod.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[postalAddressType](../resources/postaladdresstype.md)||
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
|shipmentMethodId|Guid||
|taxAreaDisplayName|String||
|taxAreaId|Guid||
|taxLiable|Boolean||
|taxRegistrationNumber|String||
|type|String||
|website|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)||
|paymentMethod|[paymentMethod](../resources/paymentmethod.md)||
|paymentTerm|[paymentTerm](../resources/paymentterm.md)||
|picture|[picture](../resources/picture.md) collection||
|shipmentMethod|[shipmentMethod](../resources/shipmentmethod.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customer",
  "id": "String (identifier)",
  "number": "String",
  "displayName": "String",
  "type": "String",
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
  "taxLiable": true,
  "taxAreaId": "Guid",
  "taxAreaDisplayName": "String",
  "taxRegistrationNumber": "String",
  "currencyId": "Guid",
  "currencyCode": "String",
  "paymentTermsId": "Guid",
  "shipmentMethodId": "Guid",
  "paymentMethodId": "Guid",
  "blocked": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

