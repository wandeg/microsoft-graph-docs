---
title: "List operations"
description: "Get the teamsAsyncOperations from the operations navigation property."
author: "**TODO: Provide Github Name**"
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
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsAsyncOperation](../resources/teamsasyncoperation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_teamsasyncoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/operations
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsasyncoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsAsyncOperation",
      "id": "f499dbba-dbba-f499-badb-99f4badb99f4",
      "operationType": "String",
      "createdDateTime": "2016-12-31T23:56:51.3342982+03:00",
      "status": "String",
      "lastActionDateTime": "2017-01-01T00:02:31.8410313+03:00",
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

