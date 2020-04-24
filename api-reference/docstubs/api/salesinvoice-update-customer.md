---
title: "Update customer"
description: "Update the properties of a customer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update customer

Namespace: microsoft.graph

Update the properties of a customer object.

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
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/customer
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `200 OK` response code and an updated [customer](../resources/customer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_customer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/customer
Content-Type: application/json
Content-length: 1013

{
  "@odata.type": "#microsoft.graph.customer",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryLetterCode": "Country Letter Code value",
    "postalCode": "Postal Code value"
  },
  "phoneNumber": "Phone Number value",
  "email": "Email value",
  "website": "Website value",
  "taxLiable": true,
  "taxAreaId": "79fa183e-183e-79fa-3e18-fa793e18fa79",
  "taxAreaDisplayName": "Tax Area Display Name value",
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
  "shipmentMethodId": "f3ea0115-0115-f3ea-1501-eaf31501eaf3",
  "paymentMethodId": "52b281a7-81a7-52b2-a781-b252a781b252",
  "blocked": "Blocked value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.customer",
  "id": "71af09c2-09c2-71af-c209-af71c209af71",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryLetterCode": "Country Letter Code value",
    "postalCode": "Postal Code value"
  },
  "phoneNumber": "Phone Number value",
  "email": "Email value",
  "website": "Website value",
  "taxLiable": true,
  "taxAreaId": "79fa183e-183e-79fa-3e18-fa793e18fa79",
  "taxAreaDisplayName": "Tax Area Display Name value",
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
  "shipmentMethodId": "f3ea0115-0115-f3ea-1501-eaf31501eaf3",
  "paymentMethodId": "52b281a7-81a7-52b2-a781-b252a781b252",
  "blocked": "Blocked value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

