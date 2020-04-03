---
title: "Get roleScopeTag"
description: "Read properties and relationships of the roleScopeTag object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get roleScopeTag

Namespace: microsoft.graph

Read properties and relationships of the [roleScopeTag](../resources/rolescopetag.md) object.

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
GET /deviceManagement/roleScopeTags/{roleScopeTagId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [roleScopeTag](../resources/rolescopetag.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_rolescopetag"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": {
    "@odata.type": "#microsoft.graph.roleScopeTag",
    "id": "9c99b9d3-b9d3-9c99-d3b9-999cd3b9999c",
    "displayName": "Display Name value",
    "description": "Description value",
    "isBuiltIn": true
  }
}
```

