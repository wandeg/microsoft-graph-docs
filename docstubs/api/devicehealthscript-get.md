---
title: "Get deviceHealthScript"
description: "Read properties and relationships of the deviceHealthScript object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceHealthScript

Namespace: microsoft.graph

Read properties and relationships of the [deviceHealthScript](../resources/devicehealthscript.md) object.

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
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
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
If successful, this method returns a `200 OK` response code and [deviceHealthScript](../resources/devicehealthscript.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicehealthscript"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 804

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScript",
    "id": "a58a01e7-01e7-a58a-e701-8aa5e7018aa5",
    "publisher": "Publisher value",
    "version": "Version value",
    "displayName": "Display Name value",
    "description": "Description value",
    "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
    "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "runAsAccount": "String",
    "enforceSignatureCheck": true,
    "runAs32Bit": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "isGlobalScript": true,
    "highestAvailableVersion": "Highest Available Version value"
  }
}
```

