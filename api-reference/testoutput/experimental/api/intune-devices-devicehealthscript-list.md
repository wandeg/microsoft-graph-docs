---
title: "List deviceHealthScripts"
description: "List properties and relationships of the deviceHealthScript objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceHealthScripts

Namespace: microsoft.graph

List properties and relationships of the [deviceHealthScript](../resources/devicehealthscript.md) objects.

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
GET /deviceManagement/deviceHealthScripts
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScript](../resources/devicehealthscript.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicehealthscript"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/deviceHealthScripts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicehealthscript)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 753

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScript",
      "id": "aa148d30-8d30-aa14-308d-14aa308d14aa",
      "publisher": "Publisher value",
      "version": "Version value",
      "displayName": "Display Name value",
      "description": "Description value",
      "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
      "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "runAsAccount": "String",
      "enforceSignatureCheck": true,
      "runAs32Bit": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```

