---
title: "servicePrincipal: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# delta

Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

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
GET /servicePrincipals/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [servicePrincipal](../resources/microsoft.directoryservices-serviceprincipal.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delta"
}
-->
``` http
GET https://graph.microsoft.com/changelog/servicePrincipals/delta
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.directoryservices.serviceprincipal)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.servicePrincipal",
      "id": "f1245539-5539-f124-3955-24f1395524f1",
      "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
      "accountEnabled": true,
      "addIns": [
        {
          "@odata.type": "Microsoft.DirectoryServices.addIn"
        }
      ],
      "alternativeNames": [
        "Alternative Names value"
      ],
      "api": {
        "@odata.type": "Microsoft.DirectoryServices.apiServicePrincipal"
      },
      "appDisplayName": "App Display Name value",
      "appId": "App Id value",
      "applicationTemplateId": "Application Template Id value",
      "appOwnerOrganizationId": "645cf9c9-f9c9-645c-c9f9-5c64c9f95c64",
      "appRoleAssignmentRequired": true,
      "appRoles": [
        {
          "@odata.type": "Microsoft.DirectoryServices.appRole"
        }
      ],
      "displayName": "Display Name value",
      "errorUrl": "https://example.com/errorUrl/",
      "hasPermissionClassifications": true,
      "homepage": "Homepage value",
      "info": {
        "@odata.type": "Microsoft.DirectoryServices.informationalUrl"
      },
      "keyCredentials": [
        {
          "@odata.type": "Microsoft.DirectoryServices.keyCredential"
        }
      ],
      "loginUrl": "https://example.com/loginUrl/",
      "logoutUrl": "https://example.com/logoutUrl/",
      "notificationEmailAddresses": [
        "Notification Email Addresses value"
      ],
      "publishedPermissionScopes": [
        {
          "@odata.type": "Microsoft.DirectoryServices.permissionScope"
        }
      ],
      "passwordCredentials": [
        {
          "@odata.type": "Microsoft.DirectoryServices.passwordCredential"
        }
      ],
      "preferredTokenSigningKeyEndDateTime": "2016-12-31T23:59:36.1296382+00:00",
      "preferredTokenSigningKeyThumbprint": "Preferred Token Signing Key Thumbprint value",
      "preferredSingleSignOnMode": "Preferred Single Sign On Mode value",
      "publisherName": "Publisher Name value",
      "replyUrls": [
        "Reply Urls value"
      ],
      "samlMetadataUrl": "https://example.com/samlMetadataUrl/",
      "samlSingleSignOnSettings": {
        "@odata.type": "Microsoft.DirectoryServices.samlSingleSignOnSettings"
      },
      "servicePrincipalNames": [
        "Service Principal Names value"
      ],
      "servicePrincipalType": "Service Principal Type value",
      "signInAudience": "Sign In Audience value",
      "tags": [
        "Tags value"
      ],
      "tokenEncryptionKeyId": "992a9363-9363-992a-6393-2a9963932a99"
    }
  ]
}
```

