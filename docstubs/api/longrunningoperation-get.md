---
title: "Get longRunningOperation"
description: "Read properties and relationships of the longRunningOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get longRunningOperation

Namespace: microsoft.graph

Read properties and relationships of the [longRunningOperation](../resources/longrunningoperation.md) object.

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
GET /me/authentication/operations/{longRunningOperationId}
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
If successful, this method returns a `200 OK` response code and [longRunningOperation](../resources/longrunningoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_longrunningoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/operations/{longRunningOperationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.longRunningOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "value": {
    "@odata.type": "#microsoft.graph.longRunningOperation",
    "id": "70cd0ba0-0ba0-70cd-a00b-cd70a00bcd70",
    "createdDateTime": "2017-01-01T00:00:01.0610721+03:00",
    "lastActionDateTime": "2017-01-01T00:02:09.4916918+03:00",
    "status": "String",
    "statusDetail": "Status Detail value",
    "resourceLocation": "Resource Location value"
  }
}
```

