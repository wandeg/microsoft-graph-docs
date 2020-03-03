---
title: "List privilegedRoles"
description: "List properties and relationships of the privilegedRole objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List privilegedRoles

List properties and relationships of the [privilegedRole](../resources/privilegedrole.md) objects.

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
GET /privilegedRoles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/privilegedRoles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedrole)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 175

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedRole",
      "id": "6f5192e5-92e5-6f51-e592-516fe592516f",
      "name": "Name value"
    }
  ]
}
```

