---
title: "List oauth2PermissionGrants"
description: "Get the oAuth2PermissionGrants from the oauth2PermissionGrants navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List oauth2PermissionGrants

Namespace: microsoft.graph

Get the oAuth2PermissionGrants from the oauth2PermissionGrants navigation property.

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
GET /servicePrincipals/{servicePrincipalsId}/oauth2PermissionGrants
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrant"
}
-->
``` http
GET https://graph.microsoft.com/localtest/servicePrincipals/{servicePrincipalsId}/oauth2PermissionGrants
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
      "id": "4dea3746-3746-4dea-4637-ea4d4637ea4d",
      "clientId": "Client Id value",
      "consentType": "Consent Type value",
      "expiryTime": "2016-12-31T23:58:12.6684613+03:00",
      "principalId": "Principal Id value",
      "resourceId": "Resource Id value",
      "scope": "Scope value",
      "startTime": "2017-01-01T00:02:49.6370207+03:00"
    }
  ]
}
```

