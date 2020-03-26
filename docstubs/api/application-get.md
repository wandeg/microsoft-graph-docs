---
title: "Get application"
description: "Read properties and relationships of the application object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get application

Namespace: microsoft.graph

Read properties and relationships of the [application](../resources/application.md) object.

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
GET /applications/{applicationsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [application](../resources/application.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_application"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5216

{
  "value": {
    "@odata.type": "#microsoft.graph.application",
    "id": "53ba3be2-3be2-53ba-e23b-ba53e23bba53",
    "deletedDateTime": "2016-12-31T23:56:48.9746736+00:00",
    "addIns": [
      {
        "@odata.type": "microsoft.graph.addIn",
        "id": "c28040e5-40e5-c280-e540-80c2e54080c2",
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
    "api": {
      "@odata.type": "microsoft.graph.apiApplication",
      "acceptMappedClaims": true,
      "knownClientApplications": [
        "c775da20-da20-c775-20da-75c720da75c7"
      ],
      "preAuthorizedApplications": [
        {
          "@odata.type": "microsoft.graph.preAuthorizedApplication",
          "appId": "App Id value",
          "delegatedPermissionIds": [
            "Delegated Permission Ids value"
          ]
        }
      ],
      "requestedAccessTokenVersion": 11,
      "oauth2PermissionScopes": [
        {
          "@odata.type": "microsoft.graph.permissionScope",
          "adminConsentDescription": "Admin Consent Description value",
          "adminConsentDisplayName": "Admin Consent Display Name value",
          "isEnabled": true,
          "origin": "Origin value",
          "userConsentDescription": "User Consent Description value",
          "userConsentDisplayName": "User Consent Display Name value"
        }
      ]
    },
    "appId": "App Id value",
    "applicationTemplateId": "Application Template Id value",
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
    "isFallbackPublicClient": true,
    "identifierUris": [
      "Identifier Uris value"
    ],
    "createdDateTime": "2016-12-31T23:58:54.5578393+00:00",
    "publicClient": {
      "@odata.type": "microsoft.graph.publicClientApplication",
      "redirectUris": [
        "Redirect Uris value"
      ]
    },
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
        "endDateTime": "2017-01-01T00:02:46.3269187+00:00",
        "keyId": "2cdf9d77-9d77-2cdf-779d-df2c779ddf2c",
        "startDateTime": "2016-12-31T23:57:46.9348086+00:00",
        "usage": "Usage value",
        "key": "a2V5"
      }
    ],
    "logo": "Stream",
    "oauth2RequirePostResponse": true,
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
    "tokenEncryptionKeyId": "a51bd40b-d40b-a51b-0bd4-1ba50bd41ba5",
    "web": {
      "@odata.type": "microsoft.graph.webApplication",
      "homePageUrl": "https://example.com/homePageUrl/",
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

