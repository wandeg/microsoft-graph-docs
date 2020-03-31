---
title: "makePermanent"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# makePermanent

Namespace: microsoft.graph



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
POST /privilegedRoleAssignments/{privilegedRoleAssignmentsId}/makePermanent
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|reason|String||
|ticketNumber|String||
|ticketSystem|String||



## Response
If successful, this action returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makepermanent"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{privilegedRoleAssignmentsId}/makePermanent

Content-type: application/json
Content-length: 116

{
  "reason": "Reason value",
  "ticketNumber": "Ticket Number value",
  "ticketSystem": "Ticket System value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 337

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
    "id": "8a453401-3401-8a45-0134-458a0134458a",
    "userId": "User Id value",
    "roleId": "Role Id value",
    "isElevated": true,
    "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
    "resultMessage": "Result Message value"
  }
}
```

