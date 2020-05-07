---
title: "List deviceManagementScripts"
description: "Get the deviceManagementScripts from the deviceManagementScripts navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceManagementScripts

Namespace: microsoft.graph

Get the deviceManagementScripts from the deviceManagementScripts navigation property.

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
GET /deviceManagement/deviceManagementScripts
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/devicemanagementscript.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementscript"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementscript)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScript",
      "id": "a5dd2be4-2be4-a5dd-e42b-dda5e42bdda5",
      "enforceSignatureCheck": "Boolean",
      "runAs32Bit": "Boolean",
      "displayName": "String",
      "description": "String",
      "scriptContent": "Binary",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "runAsAccount": "String",
      "fileName": "String",
      "roleScopeTagIds": [
        "String"
      ]
    }
  ]
}
```

