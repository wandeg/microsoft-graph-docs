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
GET /servicePrincipals/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delta"
}
-->
``` http
GET https://graph.microsoft.com/localtest/servicePrincipals/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.serviceprincipal)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1802

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "0cf3ca8d-ca8d-0cf3-8dca-f30c8dcaf30c",
      "deletedDateTime": "2016-12-31T23:57:45.8652256+03:00",
      "accountEnabled": true,
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn"
        }
      ],
      "appDisplayName": "App Display Name value",
      "appId": "App Id value",
      "applicationTemplateId": "Application Template Id value",
      "appOwnerOrganizationId": "6c64b8b7-b8b7-6c64-b7b8-646cb7b8646c",
      "appRoleAssignmentRequired": true,
      "appRoles": [
        {
          "@odata.type": "microsoft.graph.appRole"
        }
      ],
      "displayName": "Display Name value",
      "homepage": "Homepage value",
      "keyCredentials": [
        {
          "@odata.type": "microsoft.graph.keyCredential"
        }
      ],
      "info": {
        "@odata.type": "microsoft.graph.informationalUrl"
      },
      "logoutUrl": "https://example.com/logoutUrl/",
      "notificationEmailAddresses": [
        "Notification Email Addresses value"
      ],
      "publishedPermissionScopes": [
        {
          "@odata.type": "microsoft.graph.permissionScope"
        }
      ],
      "passwordCredentials": [
        {
          "@odata.type": "microsoft.graph.passwordCredential"
        }
      ],
      "preferredTokenSigningKeyThumbprint": "Preferred Token Signing Key Thumbprint value",
      "publisherName": "Publisher Name value",
      "replyUrls": [
        "Reply Urls value"
      ],
      "samlMetadataUrl": "https://example.com/samlMetadataUrl/",
      "servicePrincipalNames": [
        "Service Principal Names value"
      ],
      "tags": [
        "Tags value"
      ]
    }
  ]
}
```

