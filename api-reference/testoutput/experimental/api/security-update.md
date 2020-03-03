---
title: "Update security"
description: "Update the properties of a security object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update security

Namespace: microsoft.graph

Update the properties of a [security](../resources/security.md) object.

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
PATCH /Security
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [security](../resources/security.md) object.

The following table shows the properties that are required when you create the [security](../resources/security.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|providerStatus|[securityProviderStatus](../resources/securityproviderstatus.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [security](../resources/security.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_security"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/Security
Content-type: application/json
Content-length: 320

{
  "@odata.type": "#microsoft.graph.security",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 369

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
```

