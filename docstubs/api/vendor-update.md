---
title: "Update vendor"
description: "Update the properties of a vendor object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update vendor

Namespace: microsoft.graph

Update the properties of a [vendor](../resources/vendor.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [vendor](../resources/vendor.md) object.

The following table shows the properties that are required when you create the [vendor](../resources/vendor.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|displayName|String||
|address|[postalAddressType](../resources/postaladdresstype.md)||
|phoneNumber|String||
|email|String||
|website|String||
|taxRegistrationNumber|String||
|currencyId|Guid||
|currencyCode|String||
|paymentTermsId|Guid||
|paymentMethodId|Guid||
|taxLiable|Boolean||
|blocked|String||
|balance|Decimal||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [vendor](../resources/vendor.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_vendor"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/vendors/{vendorId}
Content-type: application/json
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
  "currencyId": "5718300d-300d-5718-0d30-18570d301857",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "ee8dd96e-d96e-ee8d-6ed9-8dee6ed98dee",
  "paymentMethodId": "9309ed2d-ed2d-9309-2ded-09932ded0993",
  "taxLiable": true,
  "blocked": "Blocked value",
  "balance": "4.2"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 945

{
  "@odata.type": "#microsoft.graph.vendor",
  "id": "fe0945c8-45c8-fe09-c845-09fec84509fe",
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
  "currencyId": "5718300d-300d-5718-0d30-18570d301857",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "ee8dd96e-d96e-ee8d-6ed9-8dee6ed98dee",
  "paymentMethodId": "9309ed2d-ed2d-9309-2ded-09932ded0993",
  "taxLiable": true,
  "blocked": "Blocked value",
  "balance": "4.2",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
}
```

