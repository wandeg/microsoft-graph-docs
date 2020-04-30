---
title: "Update oAuth2PermissionGrant"
description: "Update the properties of a oAuth2PermissionGrant object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update oAuth2PermissionGrant

Namespace: Microsoft.DirectoryServices

Update the properties of a [oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md) object.

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
PATCH /oauth2PermissionGrants/{oauth2PermissionGrantsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md) object.

The following table shows the properties that are required when you create the [oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md).

|Property|Type|Description|
|:---|:---|:---|
|clientId|String|**TODO: Add Description**|
|consentType|String|**TODO: Add Description**|
|expiryTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|principalId|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|scope|String|**TODO: Add Description**|
|startTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [oAuth2PermissionGrant](../resources/microsoft.directoryservices-oauth2permissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_oauth2permissiongrant"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/oauth2PermissionGrants/{oauth2PermissionGrantsId}
Content-Type: application/json
Content-length: 361

{
  "@odata.type": "#Microsoft.DirectoryServices.oAuth2PermissionGrant",
  "clientId": "Client Id value",
  "consentType": "Consent Type value",
  "expiryTime": "2017-01-01T00:03:20.4286312+00:00",
  "principalId": "Principal Id value",
  "resourceId": "Resource Id value",
  "scope": "Scope value",
  "startTime": "2016-12-31T23:56:55.3488457+00:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

