---
title: "Get deviceHealthScript"
description: "Read the properties and relationships of a deviceHealthScript object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get deviceHealthScript

Namespace: microsoft.graph

Read the properties and relationships of a [deviceHealthScript](../resources/devicehealthscript.md) object.

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
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [deviceHealthScript](../resources/devicehealthscript.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicehealthscript"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScript",
    "id": "8fe3e3c4-e3c4-8fe3-c4e3-e38fc4e3e38f",
    "publisher": "Publisher value",
    "version": "Version value",
    "displayName": "Display Name value",
    "description": "Description value",
    "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
    "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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

