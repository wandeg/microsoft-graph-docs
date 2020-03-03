---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta



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
GET /oauth2PermissionGrants/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/oauth2PermissionGrants/delta
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
Content-Length: 467

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
      "id": "b4971c0a-1c0a-b497-0a1c-97b40a1c97b4",
      "clientId": "Client Id value",
      "consentType": "Consent Type value",
      "expiryTime": "2017-01-01T00:01:52.1150286+03:00",
      "principalId": "Principal Id value",
      "resourceId": "Resource Id value",
      "scope": "Scope value",
      "startTime": "2016-12-31T23:59:41.6500596+03:00"
    }
  ]
}
```

