---
title: "export"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# export

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
GET /governanceRoleAssignments/export
GET /privilegedAccess/{privilegedAccessId}/roleAssignments/export
GET /governanceResources/{governanceResourcesId}/roleAssignments/export
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/export
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a String collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "governanceroleassignment_export"
}
-->
``` http
GET https://graph.microsoft.com/beta/governanceRoleAssignments/export
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(edm.string)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 43

{
  "value": [
    "Export value"
  ]
}
```

