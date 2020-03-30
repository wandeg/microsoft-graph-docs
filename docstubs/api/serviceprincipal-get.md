---
title: "Get servicePrincipal"
description: "Read properties and relationships of the servicePrincipal object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get servicePrincipal

Namespace: microsoft.graph

Read properties and relationships of the [servicePrincipal](../resources/serviceprincipal.md) object.

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
GET /servicePrincipals/{servicePrincipalsId}
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
If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}
-->
``` http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3811

{
  "value": {
    "@odata.type": "#microsoft.graph.servicePrincipal",
    "id": "ba3f5ba0-5ba0-ba3f-a05b-3fbaa05b3fba",
    "deletedDateTime": "2016-12-31T23:57:00.1067265+03:00",
    "accountEnabled": true,
    "addIns": [
      {
        "@odata.type": "microsoft.graph.addIn",
        "id": "174827b3-27b3-1748-b327-4817b3274817",
        "type": "Type value",
        "properties": [
          {
            "@odata.type": "microsoft.graph.keyValue",
            "key": "Key value",
            "value": "Value value"
          }
        ]
      }
    ],
    "alternativeNames": [
      "Alternative Names value"
    ],
    "appDisplayName": "App Display Name value",
    "appId": "App Id value",
    "applicationTemplateId": "Application Template Id value",
    "appOwnerOrganizationId": "25a8ac47-ac47-25a8-47ac-a82547aca825",
    "appRoleAssignmentRequired": true,
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole",
        "allowedMemberTypes": [
          "Allowed Member Types value"
        ],
        "description": "Description value",
        "displayName": "Display Name value",
        "isEnabled": true,
        "origin": "Origin value"
      }
    ],
    "displayName": "Display Name value",
    "errorUrl": "https://example.com/errorUrl/",
    "homepage": "Homepage value",
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl",
      "logoUrl": "https://example.com/logoUrl/",
      "marketingUrl": "https://example.com/marketingUrl/",
      "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
      "supportUrl": "https://example.com/supportUrl/",
      "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
    },
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential",
        "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
        "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
        "keyId": "69850448-0448-6985-4804-856948048569",
        "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
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
        "@odata.type": "microsoft.graph.permissionScope",
        "adminConsentDescription": "Admin Consent Description value",
        "adminConsentDisplayName": "Admin Consent Display Name value",
        "userConsentDescription": "User Consent Description value",
        "userConsentDisplayName": "User Consent Display Name value"
      }
    ],
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential",
        "secretText": "Secret Text value",
        "hint": "Hint value"
      }
    ],
    "preferredTokenSigningKeyEndDateTime": "2016-12-31T23:56:31.924748+03:00",
    "preferredTokenSigningKeyThumbprint": "Preferred Token Signing Key Thumbprint value",
    "preferredSingleSignOnMode": "Preferred Single Sign On Mode value",
    "publisherName": "Publisher Name value",
    "replyUrls": [
      "Reply Urls value"
    ],
    "samlMetadataUrl": "https://example.com/samlMetadataUrl/",
    "samlSingleSignOnSettings": {
      "@odata.type": "microsoft.graph.samlSingleSignOnSettings",
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
    "tokenEncryptionKeyId": "db740ce5-0ce5-db74-e50c-74dbe50c74db"
  }
}
```

