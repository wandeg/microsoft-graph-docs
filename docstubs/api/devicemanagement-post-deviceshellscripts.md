---
title: "Add deviceShellScripts"
description: "Add deviceShellScripts by posting to the deviceShellScripts collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceShellScripts

Namespace: microsoft.graph

Add deviceShellScripts by posting to the deviceShellScripts collection.

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
POST /deviceManagement/deviceShellScripts/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceShellScript](../resources/deviceshellscript.md) object.

The following table shows the properties that are required when you create the [deviceShellScript](../resources/deviceshellscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|executionFrequency|Duration||
|retryCount|Int32||
|blockExecutionNotifications|Boolean||
|displayName|String||
|description|String||
|scriptContent|Binary||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|runAsAccount|Enumeration| Possible values are: `system`, `user`.|
|fileName|String||
|roleScopeTagIds|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/deviceshellscript.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceshellscript_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
Content-type: application/json
Content-length: 410

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT3M4.225773S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "String",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceshellscript"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 582

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "id": "2571e462-e462-2571-62e4-712562e47125",
  "executionFrequency": "PT3M4.225773S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
  "runAsAccount": "String",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

