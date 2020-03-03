---
title: "Get contract"
description: "Read properties and relationships of the contract object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get contract

Read properties and relationships of the [contract](../resources/contract.md) object.

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
GET /contracts/{contractsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [contract](../resources/contract.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_contract"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/contracts/{contractsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 383

{
  "value": {
    "@odata.type": "#microsoft.graph.contract",
    "id": "f721d838-d838-f721-38d8-21f738d821f7",
    "deletedDateTime": "2017-01-01T00:02:13.7092325+03:00",
    "contractType": "Contract Type value",
    "customerId": "b0dfea4b-ea4b-b0df-4bea-dfb04beadfb0",
    "defaultDomainName": "Default Domain Name value",
    "displayName": "Display Name value"
  }
}
```

