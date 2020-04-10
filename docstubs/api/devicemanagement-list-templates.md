---
title: "List templates"
description: "Get the deviceManagementTemplates from the templates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List templates

Namespace: microsoft.graph

Get the deviceManagementTemplates from the templates navigation property.

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
GET /deviceManagement/templates
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
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTemplate](../resources/devicemanagementtemplate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementtemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTemplate",
      "id": "8ac6b9fb-b9fb-8ac6-fbb9-c68afbb9c68a",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11,
      "templateType": "String",
      "platformType": "String",
      "publishedDateTime": "2016-12-31T23:56:28.3946732+00:00"
    }
  ]
}
```

