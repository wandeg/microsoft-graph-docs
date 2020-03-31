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
|Name|Description|
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
GET https://graph.microsoft.com/beta/servicePrincipals/delta
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
Content-Length: 2437

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "3dc1b9da-b9da-3dc1-dab9-c13ddab9c13d",
      "deletedDateTime": "2016-12-31T23:59:31.2455853+03:00",
      "accountEnabled": true,
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn"
        }
      ],
      "alternativeNames": [
        "Alternative Names value"
      ],
      "appDisplayName": "App Display Name value",
      "appId": "App Id value",
      "applicationTemplateId": "Application Template Id value",
      "appOwnerOrganizationId": "c80077c2-77c2-c800-c277-00c8c27700c8",
      "appRoleAssignmentRequired": true,
      "appRoles": [
        {
          "@odata.type": "microsoft.graph.appRole"
        }
      ],
      "displayName": "Display Name value",
      "errorUrl": "https://example.com/errorUrl/",
      "homepage": "Homepage value",
      "info": {
        "@odata.type": "microsoft.graph.informationalUrl"
      },
      "keyCredentials": [
        {
          "@odata.type": "microsoft.graph.keyCredential"
        }
      ],
      "loginUrl": "https://example.com/loginUrl/",
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
      "preferredTokenSigningKeyEndDateTime": "2016-12-31T23:59:29.3573763+03:00",
      "preferredTokenSigningKeyThumbprint": "Preferred Token Signing Key Thumbprint value",
      "preferredSingleSignOnMode": "Preferred Single Sign On Mode value",
      "publisherName": "Publisher Name value",
      "replyUrls": [
        "Reply Urls value"
      ],
      "samlMetadataUrl": "https://example.com/samlMetadataUrl/",
      "samlSingleSignOnSettings": {
        "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
      },
      "servicePrincipalNames": [
        "Service Principal Names value"
      ],
      "servicePrincipalType": "Service Principal Type value",
      "signInAudience": "Sign In Audience value",
      "tags": [
        "Tags value"
      ],
      "tokenEncryptionKeyId": "92a103ee-03ee-92a1-ee03-a192ee03a192"
    }
  ]
}
```

