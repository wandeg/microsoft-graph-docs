---
title: "List deviceShellScripts"
description: "List properties and relationships of the deviceShellScript objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceShellScripts

Namespace: microsoft.graph

List properties and relationships of the [deviceShellScript](../resources/deviceshellscript.md) objects.

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
GET /deviceManagement/deviceShellScripts
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceShellScript](../resources/deviceshellscript.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceshellscript"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/deviceShellScripts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceshellscript)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceShellScript",
      "id": "692bfe8a-fe8a-692b-8afe-2b698afe2b69",
      "displayName": "Display Name value",
      "description": "Description value",
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "runAsAccount": "String",
      "fileName": "File Name value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```

