---
title: "Update oAuth2PermissionGrant"
description: "Update the properties of a oAuth2PermissionGrant object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update oAuth2PermissionGrant

Namespace: microsoft.graph

Update the properties of a [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

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
PATCH /oauth2PermissionGrants/{oauth2PermissionGrantsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

The following table shows the properties that are required when you create the [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|clientId|String||
|consentType|String||
|expiryTime|DateTimeOffset||
|principalId|String||
|resourceId|String||
|scope|String||
|startTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_oauth2permissiongrant"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/oauth2PermissionGrants/{oauth2PermissionGrantsId}
Content-type: application/json
Content-length: 348

{
  "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
  "clientId": "Client Id value",
  "consentType": "Consent Type value",
  "expiryTime": "2016-12-31T23:57:53.1961406+03:00",
  "principalId": "Principal Id value",
  "resourceId": "Resource Id value",
  "scope": "Scope value",
  "startTime": "2017-01-01T00:00:02.049548+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
  "id": "c92b3b6a-3b6a-c92b-6a3b-2bc96a3b2bc9",
  "clientId": "Client Id value",
  "consentType": "Consent Type value",
  "expiryTime": "2016-12-31T23:57:53.1961406+03:00",
  "principalId": "Principal Id value",
  "resourceId": "Resource Id value",
  "scope": "Scope value",
  "startTime": "2017-01-01T00:00:02.049548+03:00"
}
```

