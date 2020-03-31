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
    "id": "c7eda95a-a95a-c7ed-5aa9-edc75aa9edc7",
    "deletedDateTime": "2016-12-31T23:56:41.707717+03:00",
    "accountEnabled": true,
    "addIns": [
      {
        "@odata.type": "microsoft.graph.addIn",
        "id": "929cad84-ad84-929c-84ad-9c9284ad9c92",
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
    "appOwnerOrganizationId": "3db7a8bc-a8bc-3db7-bca8-b73dbca8b73d",
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
        "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
        "keyId": "9500dc0c-dc0c-9500-0cdc-00950cdc0095",
        "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
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
    "preferredTokenSigningKeyEndDateTime": "2017-01-01T00:03:12.8300507+03:00",
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
    "tokenEncryptionKeyId": "f9c8988f-988f-f9c8-8f98-c8f98f98c8f9"
  }
}
```

