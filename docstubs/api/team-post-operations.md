---
title: "Create operations"
description: "Create a new operations object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create operations

Namespace: microsoft.graph

Create a new operations object.

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
POST /teams/{teamsId}/operations
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/operations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.

The following table shows the properties that are required when you create the [teamsAsyncOperation](../resources/teamsasyncoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|operationType|teamsAsyncOperationType|**TODO: Add Description**. Possible values are: `invalid`, `cloneTeam`, `archiveTeam`, `unarchiveTeam`, `createTeam`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|status|teamsAsyncOperationStatus|**TODO: Add Description**. Possible values are: `invalid`, `notStarted`, `inProgress`, `succeeded`, `failed`, `unknownFutureValue`.|
|lastActionDateTime|DateTimeOffset|**TODO: Add Description**|
|attemptsCount|Int32|**TODO: Add Description**|
|targetResourceId|String|**TODO: Add Description**|
|targetResourceLocation|String|**TODO: Add Description**|
|error|[operationError](../resources/operationerror.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_teamsasyncoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamsId}/operations
Content-Type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "operationType": "String",
  "status": "String",
  "lastActionDateTime": "2016-12-31T23:59:41.1188704+03:00",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "id": "043893a7-93a7-0438-a793-3804a7933804",
  "operationType": "String",
  "createdDateTime": "2017-01-01T00:00:27.9270493+03:00",
  "status": "String",
  "lastActionDateTime": "2016-12-31T23:59:41.1188704+03:00",
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

