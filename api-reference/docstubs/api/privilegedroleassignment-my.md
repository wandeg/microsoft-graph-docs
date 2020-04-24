---
title: "privilegedRoleAssignment: my"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# my

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /privilegedRoleAssignments/my
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedroleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
      "id": "0b252230-2230-0b25-3022-250b3022250b",
      "userId": "User Id value",
      "roleId": "Role Id value",
      "isElevated": true,
      "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
      "resultMessage": "Result Message value"
    }
  ]
}
```

