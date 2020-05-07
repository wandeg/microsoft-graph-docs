---
title: "customer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# customer resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List picture](../api/customer-list-picture.md)|[picture](../resources/picture.md) collection|Get the pictures from the picture navigation property.|
|[Create picture](../api/customer-post-picture.md)|[picture](../resources/picture.md)|Create a new picture object.|
|[Delete picture](../api/customer-delete-picture.md)|None|Delete a [picture](../resources/picture.md) object.|
|[Update picture](../api/customer-update-picture.md)|[picture](../resources/picture.md)|Update the properties of a picture object.|
|[Get picture](../api/picture-get.md)|[picture](../resources/picture.md)|Read the properties and relationships of a [picture](../resources/picture.md) object.|
|[List currency](../api/customer-list-currency.md)|[currency](../resources/currency.md) collection|Get the currencies from the currency navigation property.|
|[Create currency](../api/customer-post-currency.md)|[currency](../resources/currency.md)|Create a new currency object.|
|[Delete currency](../api/customer-delete-currency.md)|None|Delete a [currency](../resources/currency.md) object.|
|[Update currency](../api/customer-update-currency.md)|[currency](../resources/currency.md)|Update the properties of a currency object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read the properties and relationships of a [currency](../resources/currency.md) object.|
|[List paymentTerm](../api/customer-list-paymentterm.md)|[paymentTerm](../resources/paymentterm.md) collection|Get the paymentTerms from the paymentTerm navigation property.|
|[Create paymentTerm](../api/customer-post-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Create a new paymentTerm object.|
|[Delete paymentTerm](../api/customer-delete-paymentterm.md)|None|Delete a [paymentTerm](../resources/paymentterm.md) object.|
|[Update paymentTerm](../api/customer-update-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Update the properties of a paymentTerm object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read the properties and relationships of a [paymentTerm](../resources/paymentterm.md) object.|
|[List shipmentMethod](../api/customer-list-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md) collection|Get the shipmentMethods from the shipmentMethod navigation property.|
|[Create shipmentMethod](../api/customer-post-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md)|Create a new shipmentMethod object.|
|[Delete shipmentMethod](../api/customer-delete-shipmentmethod.md)|None|Delete a [shipmentMethod](../resources/shipmentmethod.md) object.|
|[Update shipmentMethod](../api/customer-update-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md)|Update the properties of a shipmentMethod object.|
|[Get shipmentMethod](../api/shipmentmethod-get.md)|[shipmentMethod](../resources/shipmentmethod.md)|Read the properties and relationships of a [shipmentMethod](../resources/shipmentmethod.md) object.|
|[List paymentMethod](../api/customer-list-paymentmethod.md)|[paymentMethod](../resources/paymentmethod.md) collection|Get the paymentMethods from the paymentMethod navigation property.|
|[Create paymentMethod](../api/customer-post-paymentmethod.md)|[paymentMethod](../resources/paymentmethod.md)|Create a new paymentMethod object.|
|[Delete paymentMethod](../api/customer-delete-paymentmethod.md)|None|Delete a [paymentMethod](../resources/paymentmethod.md) object.|
|[Update paymentMethod](../api/customer-update-paymentmethod.md)|[paymentMethod](../resources/paymentmethod.md)|Update the properties of a paymentMethod object.|
|[Get paymentMethod](../api/paymentmethod-get.md)|[paymentMethod](../resources/paymentmethod.md)|Read the properties and relationships of a [paymentMethod](../resources/paymentmethod.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
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
|shipmentMethodId|Guid|**TODO: Add Description**|
|taxAreaDisplayName|String|**TODO: Add Description**|
|taxAreaId|Guid|**TODO: Add Description**|
|taxLiable|Boolean|**TODO: Add Description**|
|taxRegistrationNumber|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|website|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)|**TODO: Add Description**|
|paymentMethod|[paymentMethod](../resources/paymentmethod.md)|**TODO: Add Description**|
|paymentTerm|[paymentTerm](../resources/paymentterm.md)|**TODO: Add Description**|
|picture|[picture](../resources/picture.md) collection|**TODO: Add Description**|
|shipmentMethod|[shipmentMethod](../resources/shipmentmethod.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "email": "String",
  "website": "String",
  "taxLiable": "Boolean",
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

