---
title: "customerPayment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# customerPayment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List customer](../api/customerpayment-list-customer.md)|[customer](../resources/customer.md) collection|Get the customers from the customer navigation property.|
|[Create customer](../api/customerpayment-post-customer.md)|[customer](../resources/customer.md)|Create a new customer object.|
|[Delete customer](../api/customerpayment-delete-customer.md)|None|Delete a [customer](../resources/customer.md) object.|
|[Update customer](../api/customerpayment-update-customer.md)|[customer](../resources/customer.md)|Update the properties of a customer object.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read the properties and relationships of a [customer](../resources/customer.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|amount|Decimal|**TODO: Add Description**|
|appliesToInvoiceId|Guid|**TODO: Add Description**|
|appliesToInvoiceNumber|String|**TODO: Add Description**|
|comment|String|**TODO: Add Description**|
|contactId|String|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|customerNumber|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|documentNumber|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lineNumber|Int32|**TODO: Add Description**|
|postingDate|Date|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|customer|[customer](../resources/customer.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "lineNumber": "Integer",
  "customerId": "Guid",
  "customerNumber": "String",
  "contactId": "String",
  "postingDate": "Date",
  "documentNumber": "String",
  "externalDocumentNumber": "String",
  "amount": "Decimal",
  "appliesToInvoiceId": "Guid",
  "appliesToInvoiceNumber": "String",
  "description": "String",
  "comment": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

