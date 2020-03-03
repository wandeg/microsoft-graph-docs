---
title: "List securityBaselineTemplates"
description: "List properties and relationships of the securityBaselineTemplate objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List securityBaselineTemplates

Namespace: microsoft.graph

List properties and relationships of the [securityBaselineTemplate](../resources/securitybaselinetemplate.md) objects.

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
GET ** Collection URI for microsoft.graph.securityBaselineTemplate not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [securityBaselineTemplate](../resources/securitybaselinetemplate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_securitybaselinetemplate"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.securityBaselineTemplate not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.securitybaselinetemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineTemplate",
      "id": "c06e3ed2-3ed2-c06e-d23e-6ec0d23e6ec0",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11,
      "templateType": "String",
      "platformType": "String",
      "publishedDateTime": "2016-12-31T23:58:08.6084682+03:00"
    }
  ]
}
```

