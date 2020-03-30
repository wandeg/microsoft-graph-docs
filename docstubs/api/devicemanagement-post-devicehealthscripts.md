---
title: "Add deviceHealthScripts"
description: "Add deviceHealthScripts by posting to the deviceHealthScripts collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceHealthScripts

Namespace: microsoft.graph

Add deviceHealthScripts by posting to the deviceHealthScripts collection.

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
POST /deviceManagement/deviceHealthScripts/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceHealthScript](../resources/devicehealthscript.md) object.

The following table shows the properties that are required when you create the [deviceHealthScript](../resources/devicehealthscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|publisher|String||
|version|String||
|displayName|String||
|description|String||
|detectionScriptContent|Binary||
|remediationScriptContent|Binary||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|runAsAccount|Enumeration| Possible values are: `system`, `user`.|
|enforceSignatureCheck|Boolean||
|runAs32Bit|Boolean||
|roleScopeTagIds|String collection||
|isGlobalScript|Boolean||
|highestAvailableVersion|String||



## Response
If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/devicehealthscript.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicehealthscript_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
Content-type: application/json
Content-length: 577

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicehealthscript"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 749

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "0cc20ad4-0ad4-0cc2-d40a-c20cd40ac20c",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value"
}
```

