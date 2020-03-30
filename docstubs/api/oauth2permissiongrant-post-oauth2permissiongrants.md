---
title: "Create oAuth2PermissionGrant"
description: "Create a new oAuth2PermissionGrant object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create oAuth2PermissionGrant

Namespace: microsoft.graph

Create a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

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
POST /oauth2PermissionGrants
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_oauth2permissiongrant_from_oauth2permissiongrants"
}
-->
``` http
POST https://graph.microsoft.com/beta/oauth2PermissionGrants
Content-type: application/json
Content-length: 348

{
  "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
  "clientId": "Client Id value",
  "consentType": "Consent Type value",
  "expiryTime": "2017-01-01T00:03:00.697683+03:00",
  "principalId": "Principal Id value",
  "resourceId": "Resource Id value",
  "scope": "Scope value",
  "startTime": "2017-01-01T00:03:19.9059331+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oauth2permissiongrant"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 397

{
  "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
  "id": "4ea3c297-c297-4ea3-97c2-a34e97c2a34e",
  "clientId": "Client Id value",
  "consentType": "Consent Type value",
  "expiryTime": "2017-01-01T00:03:00.697683+03:00",
  "principalId": "Principal Id value",
  "resourceId": "Resource Id value",
  "scope": "Scope value",
  "startTime": "2017-01-01T00:03:19.9059331+03:00"
}
```

