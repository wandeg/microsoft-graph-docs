---
title: "Get teamsAsyncOperation"
description: "Read properties and relationships of a teamsAsyncOperation object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get teamsAsyncOperation

Namespace: microsoft.graph

Read properties and relationships of a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.

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
GET /teams/{teamsId}/operations/{teamsAsyncOperationId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/operations/{teamsAsyncOperationId}
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
If successful, this method returns a `200 OK` response code and a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_teamsasyncoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/operations/{teamsAsyncOperationId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.teamsAsyncOperation",
    "id": "e0f4f5e2-f5e2-e0f4-e2f5-f4e0e2f5f4e0",
    "operationType": "String",
    "createdDateTime": "2016-12-31T23:57:54.5933585+03:00",
    "status": "String",
    "lastActionDateTime": "2016-12-31T23:59:38.4178255+03:00",
    "attemptsCount": 13,
    "targetResourceId": "Target Resource Id value",
    "targetResourceLocation": "Target Resource Location value",
    "error": {
      "@odata.type": "microsoft.graph.operationError",
      "code": "Code value",
      "message": "Message value"
    }
  }
}
```

