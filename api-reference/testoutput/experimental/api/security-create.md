---
title: "Create security"
description: "Create a new security object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create security

Namespace: microsoft.graph

Create a new [security](../resources/security.md) object.

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
POST ** Collection URI for microsoft.graph.security not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [security](../resources/security.md) object.

The following table shows the properties that are required when you create the [security](../resources/security.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|providerStatus|[securityProviderStatus](../resources/securityproviderstatus.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [security](../resources/security.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_security_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.security not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}
-->
``` http
HTTP/1.1 201 Created
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

