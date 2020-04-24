---
title: "Get application"
description: "Read the properties and relationships of an application object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get application

Namespace: microsoft.graph

Read the properties and relationships of an [application](../resources/application.md) object.

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
GET /applications/{applicationsId}
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
If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_application"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.application",
    "id": "2281d2dd-d2dd-2281-ddd2-8122ddd28122",
    "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
    "api": {
      "@odata.type": "microsoft.graph.apiApplication",
      "acceptMappedClaims": true,
      "knownClientApplications": [
        "33efe0bc-e0bc-33ef-bce0-ef33bce0ef33"
      ],
      "preAuthorizedApplications": [
        {
          "@odata.type": "microsoft.graph.preAuthorizedApplication",
          "appId": "App Id value",
          "permissionIds": [
            "Permission Ids value"
          ]
        }
      ],
      "requestedAccessTokenVersion": 11,
      "oauth2PermissionScopes": [
        {
          "@odata.type": "microsoft.graph.permissionScope",
          "adminConsentDescription": "Admin Consent Description value",
          "adminConsentDisplayName": "Admin Consent Display Name value",
          "id": "081ab855-b855-081a-55b8-1a0855b81a08",
          "isEnabled": true,
          "origin": "Origin value",
          "type": "Type value",
          "userConsentDescription": "User Consent Description value",
          "userConsentDisplayName": "User Consent Display Name value",
          "value": "Value value"
        }
      ]
    },
    "appId": "App Id value",
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole",
        "allowedMemberTypes": [
          "Allowed Member Types value"
        ],
        "description": "Description value",
        "displayName": "Display Name value"
      }
    ],
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "isFallbackPublicClient": true,
    "identifierUris": [
      "Identifier Uris value"
    ],
    "displayName": "Display Name value",
    "groupMembershipClaims": "Group Membership Claims value",
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl",
      "logoUrl": "https://example.com/logoUrl/",
      "marketingUrl": "https://example.com/marketingUrl/",
      "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
      "supportUrl": "https://example.com/supportUrl/",
      "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
    },
    "isDeviceOnlyAuthSupported": true,
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential",
        "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
        "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
        "keyId": "3378f387-f387-3378-87f3-783387f37833",
        "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
        "usage": "Usage value",
        "key": "a2V5"
      }
    ],
    "logo": "Stream",
    "optionalClaims": {
      "@odata.type": "microsoft.graph.optionalClaims",
      "idToken": [
        {
          "@odata.type": "microsoft.graph.optionalClaim",
          "name": "Name value",
          "source": "Source value",
          "essential": true,
          "additionalProperties": [
            "Additional Properties value"
          ]
        }
      ],
      "accessToken": [
        {
          "@odata.type": "microsoft.graph.optionalClaim"
        }
      ],
      "saml2Token": [
        {
          "@odata.type": "microsoft.graph.optionalClaim"
        }
      ]
    },
    "parentalControlSettings": {
      "@odata.type": "microsoft.graph.parentalControlSettings",
      "countriesBlockedForMinors": [
        "Countries Blocked For Minors value"
      ],
      "legalAgeGroupRule": "Legal Age Group Rule value"
    },
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential",
        "secretText": "Secret Text value",
        "hint": "Hint value"
      }
    ],
    "publicClient": {
      "@odata.type": "microsoft.graph.publicClientApplication",
      "redirectUris": [
        "Redirect Uris value"
      ]
    },
    "publisherDomain": "Publisher Domain value",
    "requiredResourceAccess": [
      {
        "@odata.type": "microsoft.graph.requiredResourceAccess",
        "resourceAppId": "Resource App Id value",
        "resourceAccess": [
          {
            "@odata.type": "microsoft.graph.resourceAccess"
          }
        ]
      }
    ],
    "signInAudience": "Sign In Audience value",
    "tags": [
      "Tags value"
    ],
    "tokenEncryptionKeyId": "ca3fb1e4-b1e4-ca3f-e4b1-3fcae4b13fca",
    "web": {
      "@odata.type": "microsoft.graph.webApplication",
      "homePageUrl": "https://example.com/homePageUrl/",
      "oauth2AllowImplicitFlow": true,
      "logoutUrl": "https://example.com/logoutUrl/",
      "implicitGrantSettings": {
        "@odata.type": "microsoft.graph.implicitGrantSettings",
        "enableIdTokenIssuance": true,
        "enableAccessTokenIssuance": true
      }
    }
  }
}
```

