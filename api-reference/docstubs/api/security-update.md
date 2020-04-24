---
title: "Update security"
description: "Update the properties of a security object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update security

Namespace: microsoft.graph

Update the properties of a [security](../resources/security.md) object.

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
PATCH /Security
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [security](../resources/security.md) object.

The following table shows the properties that are required when you create the [security](../resources/security.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|providerStatus|[securityProviderStatus](../resources/securityproviderstatus.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [security](../resources/security.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_security"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.security",
  "id": "a090a7df-a7df-a090-dfa7-90a0dfa790a0",
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

