---
title: "my"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# my

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
GET /privilegedRoleAssignments/my
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedroleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 365

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
      "id": "c69289b1-89b1-c692-b189-92c6b18992c6",
      "userId": "User Id value",
      "roleId": "Role Id value",
      "isElevated": true,
      "expirationDateTime": "2016-12-31T23:58:53.1230242+00:00",
      "resultMessage": "Result Message value"
    }
  ]
}
```

