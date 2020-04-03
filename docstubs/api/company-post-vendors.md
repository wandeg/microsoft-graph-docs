---
title: "Add vendors"
description: "Add vendors by posting to the vendors collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add vendors

Namespace: microsoft.graph

Add vendors by posting to the vendors collection.

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
POST /financials/companies/{companyId}/vendors/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_vendor_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/vendors
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
  "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "c1ae039b-039b-c1ae-9b03-aec19b03aec1",
  "paymentMethodId": "199aeaed-eaed-199a-edea-9a19edea9a19",
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
  "id": "895a6d40-6d40-895a-406d-5a89406d5a89",
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
  "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "c1ae039b-039b-c1ae-9b03-aec19b03aec1",
  "paymentMethodId": "199aeaed-eaed-199a-edea-9a19edea9a19",
  "taxLiable": true,
  "blocked": "Blocked value",
  "balance": "4.2",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

