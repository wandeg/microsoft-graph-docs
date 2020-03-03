---
title: "Create paymentMethod"
description: "Create a new paymentMethod object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create paymentMethod

Namespace: microsoft.graph

Create a new [paymentMethod](../resources/paymentmethod.md) object.

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
POST /financials/companies/{companyId}/paymentMethods
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [paymentMethod](../resources/paymentmethod.md) object.

The following table shows the properties that are required when you create the [paymentMethod](../resources/paymentmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [paymentMethod](../resources/paymentmethod.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_paymentmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/paymentMethods
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.paymentMethod",
  "code": "Code value",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.paymentmethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.paymentMethod",
  "id": "620d69bd-69bd-620d-bd69-0d62bd690d62",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
}
```

