---
title: "oAuth2PermissionGrant: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# delta
Namespace: microsoft.graph

**TODO: Add Description**

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
GET /oauth2PermissionGrants/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Function parameters
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/delta
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.oauth2permissiongrant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
      "id": "String (identifier)",
      "clientId": "String",
      "consentType": "String",
      "expiryTime": "String (timestamp)",
      "principalId": "String",
      "resourceId": "String",
      "scope": "String",
      "startTime": "String (timestamp)"
    }
  ]
}
```

