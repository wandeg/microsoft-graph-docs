---
title: "List securities"
description: "List properties and relationships of the security objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List securities

Namespace: microsoft.graph

List properties and relationships of the [security](../resources/security.md) objects.

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
GET ** Collection URI for microsoft.graph.security not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [security](../resources/security.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_security"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.security not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.security)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.security",
      "id": "2026c75e-c75e-2026-5ec7-26205ec72620",
      "providerStatus": [
        {
          "@odata.type": "microsoft.graph.securityProviderStatus",
          "enabled": true,
          "endpoint": "Endpoint value",
          "provider": "Provider value",
          "region": "Region value",
          "vendor": "Vendor value"
        }
      ]
    }
  ]
}
```

