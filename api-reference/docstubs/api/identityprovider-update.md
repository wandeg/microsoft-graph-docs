---
title: "Update identityProvider"
description: "Update the properties of an identityProvider object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update identityProvider

Namespace: microsoft.graph

Update the properties of an [identityProvider](../resources/identityprovider.md) object.

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
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [identityProvider](../resources/identityprovider.md) object.

The following table shows the properties that are required when you create the [identityProvider](../resources/identityprovider.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|type|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|clientId|String|**TODO: Add Description**|
|clientSecret|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [identityProvider](../resources/identityprovider.md) object in the response body.

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
  "@odata.type": "#microsoft.graph.identityProvider",
  "id": "baf9dc69-dc69-baf9-69dc-f9ba69dcf9ba",
  "type": "Type value",
  "name": "Name value",
  "clientId": "Client Id value",
  "clientSecret": "Client Secret value"
}
```

