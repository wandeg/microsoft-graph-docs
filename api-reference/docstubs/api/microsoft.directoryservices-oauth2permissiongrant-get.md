---
title: "Get oAuth2PermissionGrant"
description: "Read properties and relationships of an oAuth2PermissionGrant object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get oAuth2PermissionGrant

Namespace: Microsoft.DirectoryServices

Read properties and relationships of an [oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md) object.

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
GET /oauth2PermissionGrants/{oauth2PermissionGrantsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrant"
}
-->
``` http
GET https://graph.microsoft.com/changelog/oauth2PermissionGrants/{oauth2PermissionGrantsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.oAuth2PermissionGrant"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.oAuth2PermissionGrant",
    "clientId": "Client Id value",
    "consentType": "Consent Type value",
    "expiryTime": "2017-01-01T00:03:20.4286312+00:00",
    "id": "baf40c58-0c58-baf4-580c-f4ba580cf4ba",
    "principalId": "Principal Id value",
    "resourceId": "Resource Id value",
    "scope": "Scope value",
    "startTime": "2016-12-31T23:56:55.3488457+00:00"
  }
}
```

