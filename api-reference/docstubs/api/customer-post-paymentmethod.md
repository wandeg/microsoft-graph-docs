---
title: "Create paymentMethod"
description: "Create a new paymentMethod object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create paymentMethod

Namespace: microsoft.graph

Create a new paymentMethod object.

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
POST /financials/companies/{companyId}/customers/{customerId}/paymentMethod
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [paymentMethod](../resources/paymentmethod.md) object.

The following table shows the properties that are required when you create the [paymentMethod](../resources/paymentmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [paymentMethod](../resources/paymentmethod.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_paymentmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/customers/{customerId}/paymentMethod
Content-Type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.paymentMethod",
  "code": "Code value",
  "displayName": "Display Name value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.paymentmethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.paymentMethod",
  "id": "ae594f64-4f64-ae59-644f-59ae644f59ae",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

