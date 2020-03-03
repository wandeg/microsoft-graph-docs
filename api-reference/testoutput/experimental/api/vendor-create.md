---
title: "Create vendor"
description: "Create a new vendor object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create vendor

Namespace: microsoft.graph

Create a new [vendor](../resources/vendor.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /financials/companies/{companyId}/vendors
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [vendor](../resources/vendor.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_vendor_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/vendors
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
  "currencyId": "5323df69-df69-5323-69df-235369df2353",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "292944c5-44c5-2929-c544-2929c5442929",
  "paymentMethodId": "19caf68e-f68e-19ca-8ef6-ca198ef6ca19",
  "taxLiable": true,
  "blocked": "Blocked value",
  "balance": "4.2"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.vendor"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 945

{
  "@odata.type": "#microsoft.graph.vendor",
  "id": "aeeb9435-9435-aeeb-3594-ebae3594ebae",
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
  "currencyId": "5323df69-df69-5323-69df-235369df2353",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "292944c5-44c5-2929-c544-2929c5442929",
  "paymentMethodId": "19caf68e-f68e-19ca-8ef6-ca198ef6ca19",
  "taxLiable": true,
  "blocked": "Blocked value",
  "balance": "4.2",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
}
```

