---
title: "List servicePrincipals"
description: "Get a list of the servicePrincipal objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List servicePrincipals

Namespace: Microsoft.DirectoryServices

Get a list of the [servicePrincipal](../resources/serviceprincipal.md) objects and their properties.

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
GET /servicePrincipals
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
If successful, this method returns a `200 OK` response code and a collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}
-->
``` http
GET https://graph.microsoft.com/changelog/servicePrincipals
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
          "@odata.type": "Microsoft.DirectoryServices.addIn",
          "id": "6ce1b2dc-b2dc-6ce1-dcb2-e16cdcb2e16c",
          "type": "Type value",
          "properties": [
            {
              "@odata.type": "Microsoft.DirectoryServices.keyValue",
              "key": "Key value",
              "value": "Value value"
            }
          ]
        }
      ],
      "alternativeNames": [
        "Alternative Names value"
      ],
      "api": {
        "@odata.type": "Microsoft.DirectoryServices.apiServicePrincipal",
        "resourceSpecificApplicationPermissions": [
          {
            "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermission",
            "description": "Description value",
            "displayName": "Display Name value",
            "isEnabled": true
          }
        ]
      },
      "appDisplayName": "App Display Name value",
      "appId": "App Id value",
      "applicationTemplateId": "Application Template Id value",
      "appOwnerOrganizationId": "645cf9c9-f9c9-645c-c9f9-5c64c9f95c64",
      "appRoleAssignmentRequired": true,
      "appRoles": [
        {
          "@odata.type": "Microsoft.DirectoryServices.appRole",
          "allowedMemberTypes": [
            "Allowed Member Types value"
          ],
          "origin": "Origin value"
        }
      ],
      "displayName": "Display Name value",
      "errorUrl": "https://example.com/errorUrl/",
      "hasPermissionClassifications": true,
      "homepage": "Homepage value",
      "info": {
        "@odata.type": "Microsoft.DirectoryServices.informationalUrl",
        "logoUrl": "https://example.com/logoUrl/",
        "marketingUrl": "https://example.com/marketingUrl/",
        "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
        "supportUrl": "https://example.com/supportUrl/",
        "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
      },
      "keyCredentials": [
        {
          "@odata.type": "Microsoft.DirectoryServices.keyCredential",
          "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
          "endDateTime": "2017-01-01T00:01:58.2456509+00:00",
          "keyId": "c4860b27-0b27-c486-270b-86c4270b86c4",
          "startDateTime": "2017-01-01T00:01:26.5340071+00:00",
          "usage": "Usage value",
          "key": "a2V5"
        }
      ],
      "loginUrl": "https://example.com/loginUrl/",
      "logoutUrl": "https://example.com/logoutUrl/",
      "notificationEmailAddresses": [
        "Notification Email Addresses value"
      ],
      "publishedPermissionScopes": [
        {
          "@odata.type": "Microsoft.DirectoryServices.permissionScope",
          "adminConsentDescription": "Admin Consent Description value",
          "adminConsentDisplayName": "Admin Consent Display Name value",
          "userConsentDescription": "User Consent Description value",
          "userConsentDisplayName": "User Consent Display Name value"
        }
      ],
      "passwordCredentials": [
        {
          "@odata.type": "Microsoft.DirectoryServices.passwordCredential",
          "secretText": "Secret Text value",
          "hint": "Hint value"
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
        "@odata.type": "Microsoft.DirectoryServices.samlSingleSignOnSettings",
        "relayState": "Relay State value"
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

