---
title: "Create identityProvider"
description: "Create a new identityProvider object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create identityProvider

Namespace: microsoft.cpim.api.dataModels

Create a new [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) object.

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
POST /identityProviders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and an [identityProvider](../resources/microsoft.cpim.api.datamodels-identityprovider.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityProviders
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
  "truncated": true,
  "@odata.type": "microsoft.cpim.api.datamodels.identityprovider"
}
-->
``` http
HTTP/1.1 201 Created
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

