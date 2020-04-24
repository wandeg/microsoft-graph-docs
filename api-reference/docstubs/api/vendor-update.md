---
title: "Update vendor"
description: "Update the properties of a vendor object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update vendor

Namespace: microsoft.graph

Update the properties of a [vendor](../resources/vendor.md) object.

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
PATCH /financials/companies/{companyId}/vendors/{vendorId}
PATCH /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/vendor
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [vendor](../resources/vendor.md) object.

The following table shows the properties that are required when you create the [vendor](../resources/vendor.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|address|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|website|String|**TODO: Add Description**|
|taxRegistrationNumber|String|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|paymentMethodId|Guid|**TODO: Add Description**|
|taxLiable|Boolean|**TODO: Add Description**|
|blocked|String|**TODO: Add Description**|
|balance|Decimal|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [vendor](../resources/vendor.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_vendor"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/vendors/{vendorId}
Content-Type: application/json
Content-length: 832

{
  "@odata.type": "#microsoft.graph.vendor",
  "number": "Number value",
  "displayName": "Display Name value",
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
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
  "paymentMethodId": "52b281a7-81a7-52b2-a781-b252a781b252",
  "taxLiable": true,
  "blocked": "Blocked value",
  "balance": "4.2"
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
  "@odata.type": "#microsoft.graph.vendor",
  "id": "ac1e75d1-75d1-ac1e-d175-1eacd1751eac",
  "number": "Number value",
  "displayName": "Display Name value",
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
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
  "paymentMethodId": "52b281a7-81a7-52b2-a781-b252a781b252",
  "taxLiable": true,
  "blocked": "Blocked value",
  "balance": "4.2",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

