---
title: "List operations"
description: "Get the teamsAsyncOperations from the operations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List operations

Namespace: microsoft.graph

Get the teamsAsyncOperations from the operations navigation property.

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
GET /teams/{teamsId}/operations
GET /me/joinedGroups/{groupId}/team/operations
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
If successful, this method returns a `200 OK` response code and a collection of [teamsAsyncOperation](../resources/teamsasyncoperation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamsasyncoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/operations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsasyncoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 644

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsAsyncOperation",
      "id": "bd87503a-503a-bd87-3a50-87bd3a5087bd",
      "operationType": "String",
      "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
      "status": "String",
      "lastActionDateTime": "2016-12-31T23:59:45.6080321+03:00",
      "attemptsCount": 13,
      "targetResourceId": "Target Resource Id value",
      "targetResourceLocation": "Target Resource Location value",
      "error": {
        "@odata.type": "microsoft.graph.operationError",
        "code": "Code value",
        "message": "Message value"
      }
    }
  ]
}
```

