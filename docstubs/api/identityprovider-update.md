---
title: "Update identityProvider"
description: "Update the properties of a identityProvider object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update identityProvider

Namespace: microsoft.graph

Update the properties of a [identityProvider](../resources/identityprovider.md) object.

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
PATCH /identityProviders/{identityProvidersId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [identityProvider](../resources/identityprovider.md) object.

The following table shows the properties that are required when you create the [identityProvider](../resources/identityprovider.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String||
|name|String||
|clientId|String||
|clientSecret|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [identityProvider](../resources/identityprovider.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityProviders/{identityProvidersId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.identityProvider",
  "type": "Type value",
  "name": "Name value",
  "clientId": "Client Id value",
  "clientSecret": "Client Secret value"
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
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.identityProvider",
  "id": "998fce65-ce65-998f-65ce-8f9965ce8f99",
  "type": "Type value",
  "name": "Name value",
  "clientId": "Client Id value",
  "clientSecret": "Client Secret value"
}
```

