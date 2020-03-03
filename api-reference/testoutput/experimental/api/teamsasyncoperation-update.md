---
title: "Update teamsAsyncOperation"
description: "Update the properties of a teamsAsyncOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsAsyncOperation

Namespace: microsoft.graph

Update the properties of a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.

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
PATCH /teams/{teamsId}/operations/{teamsAsyncOperationId}
PATCH /me/joinedGroups/{groupId}/team/operations/{teamsAsyncOperationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.

The following table shows the properties that are required when you create the [teamsAsyncOperation](../resources/teamsasyncoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|operationType|Enumeration|. Possible values are: `invalid`, `cloneTeam`, `archiveTeam`, `unarchiveTeam`, `createTeam`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `invalid`, `notStarted`, `inProgress`, `succeeded`, `failed`, `unknownFutureValue`.|
|lastActionDateTime|DateTimeOffset||
|attemptsCount|Int32||
|targetResourceId|String||
|targetResourceLocation|String||
|error|[operationError](../resources/operationerror.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsAsyncOperation](../resources/teamsasyncoperation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsasyncoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/teams/{teamsId}/operations/{teamsAsyncOperationId}
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "operationType": "String",
  "status": "String",
  "lastActionDateTime": "2016-12-31T23:56:52.9868016+03:00",
  "attemptsCount": 13,
  "targetResourceId": "Target Resource Id value",
  "targetResourceLocation": "Target Resource Location value",
  "error": {
    "@odata.type": "microsoft.graph.operationError",
    "code": "Code value",
    "message": "Message value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 554

{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "id": "c350ef18-ef18-c350-18ef-50c318ef50c3",
  "operationType": "String",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "status": "String",
  "lastActionDateTime": "2016-12-31T23:56:52.9868016+03:00",
  "attemptsCount": 13,
  "targetResourceId": "Target Resource Id value",
  "targetResourceLocation": "Target Resource Location value",
  "error": {
    "@odata.type": "microsoft.graph.operationError",
    "code": "Code value",
    "message": "Message value"
  }
}
```

