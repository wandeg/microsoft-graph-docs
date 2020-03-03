---
title: "List policyBases"
description: "List properties and relationships of the policyBase objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List policyBases

Namespace: microsoft.graph

List properties and relationships of the [policyBase](../resources/policybase.md) objects.

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
GET ** Collection URI for microsoft.graph.policyBase not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [policyBase](../resources/policybase.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_policybase"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.policyBase not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.policybase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 229

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policyBase",
      "id": "e5c9f0a7-f0a7-e5c9-a7f0-c9e5a7f0c9e5",
      "description": "Description value",
      "displayName": "Display Name value"
    }
  ]
}
```

