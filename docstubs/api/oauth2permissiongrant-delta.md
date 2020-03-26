---
title: "delta"
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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.oauth2permissiongrant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 466

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
      "id": "c4570467-0467-c457-6704-57c4670457c4",
      "clientId": "Client Id value",
      "consentType": "Consent Type value",
      "expiryTime": "2016-12-31T23:59:21.9050689+03:00",
      "principalId": "Principal Id value",
      "resourceId": "Resource Id value",
      "scope": "Scope value",
      "startTime": "2017-01-01T00:01:11.772122+03:00"
    }
  ]
}
```

