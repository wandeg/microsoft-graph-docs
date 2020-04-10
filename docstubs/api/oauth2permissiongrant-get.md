---
title: "Get oAuth2PermissionGrant"
description: "Read properties and relationships of the oAuth2PermissionGrant object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get oAuth2PermissionGrant

Namespace: microsoft.graph

Read properties and relationships of the [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

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
GET /oauth2PermissionGrants/{oauth2PermissionGrantsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrant"
}
-->
``` http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{oauth2PermissionGrantsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": {
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
}
```

