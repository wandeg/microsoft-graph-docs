---
title: "Update identityProvider"
description: "Update the properties of a identityProvider object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update identityProvider

Namespace: microsoft.cpim.api.dataModels

Update the properties of a [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) object.

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
PATCH /identityProviders/{identityProvidersId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) object.

The following table shows the properties that are required when you create the [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|clientId|String|**TODO: Add Description**|
|clientSecret|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityProviders/{identityProvidersId}
Content-Type: application/json
Content-length: 198

{
  "@odata.type": "#microsoft.cpim.api.dataModels.identityProvider",
  "type": "Type value",
  "name": "Name value",
  "clientId": "Client Id value",
  "clientSecret": "Client Secret value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.identityProvider",
  "id": "60d1067f-067f-60d1-7f06-d1607f06d160",
  "type": "Type value",
  "name": "Name value",
  "clientId": "Client Id value",
  "clientSecret": "Client Secret value"
}
```

