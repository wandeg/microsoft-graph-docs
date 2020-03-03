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

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privilegedRoleAssignments/my
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}
-->
``` http
GET https://graph.microsoft.com/localtest/privilegedRoleAssignments/my
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
      "id": "59a88cae-8cae-59a8-ae8c-a859ae8ca859",
      "userId": "User Id value",
      "roleId": "Role Id value",
      "isElevated": true,
      "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
      "resultMessage": "Result Message value"
    }
  ]
}
```

