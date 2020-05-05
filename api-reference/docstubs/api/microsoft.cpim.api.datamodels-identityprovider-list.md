---
title: "List identityProviders"
description: "Get a list of the identityProvider objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List identityProviders

Namespace: microsoft.cpim.api.dataModels

Get a list of the [identityProvider](../resources/identityprovider.md) objects and their properties.

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
GET /identityProviders
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
If successful, this method returns a `200 OK` response code and a collection of [identityProvider](../resources/identityprovider.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProviders
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.cpim.api.datamodels.identityprovider)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.cpim.api.dataModels.identityProvider",
      "id": "60d1067f-067f-60d1-7f06-d1607f06d160",
      "type": "Type value",
      "name": "Name value",
      "clientId": "Client Id value",
      "clientSecret": "Client Secret value"
    }
  ]
}
```

