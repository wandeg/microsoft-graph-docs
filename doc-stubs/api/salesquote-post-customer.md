---
title: "Create customer"
description: "Create a new customer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create customer

Namespace: microsoft.graph

Create a new customer object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/customer
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [customer](../resources/customer.md) object.

The following table shows the properties that are required when you create the [customer](../resources/customer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|address|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|website|String|**TODO: Add Description**|
|taxLiable|Boolean|**TODO: Add Description**|
|taxAreaId|Guid|**TODO: Add Description**|
|taxAreaDisplayName|String|**TODO: Add Description**|
|taxRegistrationNumber|String|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|shipmentMethodId|Guid|**TODO: Add Description**|
|paymentMethodId|Guid|**TODO: Add Description**|
|blocked|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [customer](../resources/customer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_customer_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes/{salesQuoteId}/customer
Content-Type: application/json
Content-length: 566

{
  "@odata.type": "#microsoft.graph.customer",
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
  "blocked": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customer"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.customer",
  "id": "7b7faf36-af36-7b7f-36af-7f7b36af7f7b",
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

