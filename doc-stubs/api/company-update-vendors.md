---
title: "Update vendors"
description: "Update the properties of a vendors object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update vendors

Namespace: microsoft.graph

Update the properties of a vendors object.

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
PATCH /financials/companies/{companyId}/vendors
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
  "name": "update_vendors"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/vendors
Content-Type: application/json
Content-length: 478

{
  "@odata.type": "#microsoft.graph.vendor",
  "number": "String",
  "displayName": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "email": "String",
  "website": "String",
  "taxRegistrationNumber": "String",
  "currencyId": "Guid",
  "currencyCode": "String",
  "paymentTermsId": "Guid",
  "paymentMethodId": "Guid",
  "taxLiable": "Boolean",
  "blocked": "String",
  "balance": "Decimal"
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
  "id": "5edb46f3-46f3-5edb-f346-db5ef346db5e",
  "number": "String",
  "displayName": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "email": "String",
  "website": "String",
  "taxRegistrationNumber": "String",
  "currencyId": "Guid",
  "currencyCode": "String",
  "paymentTermsId": "Guid",
  "paymentMethodId": "Guid",
  "taxLiable": "Boolean",
  "blocked": "String",
  "balance": "Decimal",
  "lastModifiedDateTime": "String (timestamp)"
}
```

