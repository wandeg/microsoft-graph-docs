---
title: "Get teamsAsyncOperation"
description: "Read the properties and relationships of a teamsAsyncOperation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get teamsAsyncOperation

Namespace: microsoft.graph

Read the properties and relationships of a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.

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
GET /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/team/operations/{teamsAsyncOperationId}
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
**Note:** The response object shown here might be shortened for readability.
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
    "id": "d476e824-e824-d476-24e8-76d424e876d4",
    "operationType": "String",
    "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
    "status": "String",
    "lastActionDateTime": "2017-01-01T00:02:49.8376032+03:00",
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

