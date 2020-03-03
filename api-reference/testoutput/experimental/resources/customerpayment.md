---
title: "customerPayment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# customerPayment resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get customerPayment](../api/customerpayment-get.md)|[customerPayment](../resources/customerPayment.md)|Read properties and relationships of the [customerPayment](../resources/customerpayment.md) object.|
|[Delete customerPayment](../api/customerpayment-delete.md)|None|Deletes a [customerPayment](../resources/customerpayment.md).|
|[Update customerPayment](../api/customerpayment-update.md)|[customerPayment](../resources/customerPayment.md)|Update the properties of a [customerPayment](../resources/customerpayment.md) object.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read properties and relationships of the [customer](../resources/customer.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|amount|Decimal||
|appliesToInvoiceId|Guid||
|appliesToInvoiceNumber|String||
|comment|String||
|contactId|String||
|customerId|Guid||
|customerNumber|String||
|description|String||
|documentNumber|String||
|externalDocumentNumber|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String||
|lastModifiedDateTime|DateTimeOffset||
|lineNumber|Int32||
|postingDate|Date||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|customer|[customer](../resources/customer.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customerPayment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customerPayment",
  "id": "String (identifier)",
  "journalDisplayName": "String",
  "lineNumber": 1024,
  "customerId": "Guid",
  "customerNumber": "String",
  "contactId": "String",
  "postingDate": "Date",
  "documentNumber": "String",
  "externalDocumentNumber": "String",
  "amount": "4.2",
  "appliesToInvoiceId": "Guid",
  "appliesToInvoiceNumber": "String",
  "description": "String",
  "comment": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

