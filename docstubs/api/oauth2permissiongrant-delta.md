---
title: "oAuth2PermissionGrant: delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph



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
GET /oauth2PermissionGrants/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.oauth2permissiongrant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
      "id": "2755e639-e639-2755-39e6-552739e65527",
      "clientId": "Client Id value",
      "consentType": "Consent Type value",
      "expiryTime": "2016-12-31T23:58:21.1503209+00:00",
      "principalId": "Principal Id value",
      "resourceId": "Resource Id value",
      "scope": "Scope value",
      "startTime": "2016-12-31T23:59:26.4909337+00:00"
    }
  ]
}
```

