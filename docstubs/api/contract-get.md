---
title: "Get contract"
description: "Read properties and relationships of the contract object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get contract

Namespace: microsoft.graph

Read properties and relationships of the [contract](../resources/contract.md) object.

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
GET /contracts/{contractsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [contract](../resources/contract.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_contract"
}
-->
``` http
GET https://graph.microsoft.com/beta/contracts/{contractsId}
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
    "id": "92bbdbce-dbce-92bb-cedb-bb92cedbbb92",
    "deletedDateTime": "2016-12-31T23:58:50.3020202+00:00",
    "contractType": "Contract Type value",
    "customerId": "cc44c1a3-c1a3-cc44-a3c1-44cca3c144cc",
    "defaultDomainName": "Default Domain Name value",
    "displayName": "Display Name value"
  }
}
```

