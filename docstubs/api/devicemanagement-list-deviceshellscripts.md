---
title: "List deviceShellScripts"
description: "Get the deviceShellScripts from the deviceShellScripts navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceShellScripts

Namespace: microsoft.graph

Get the deviceShellScripts from the deviceShellScripts navigation property.

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
GET /deviceManagement/deviceShellScripts
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
If successful, this method returns a `200 OK` response code and a collection of [deviceShellScript](../resources/deviceshellscript.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceshellscript"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
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
Content-Length: 678

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceShellScript",
      "id": "133b91c2-91c2-133b-c291-3b13c2913b13",
      "executionFrequency": "-PT2M55.1453457S",
      "retryCount": 10,
      "blockExecutionNotifications": true,
      "displayName": "Display Name value",
      "description": "Description value",
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
      "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
      "runAsAccount": "String",
      "fileName": "File Name value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```

