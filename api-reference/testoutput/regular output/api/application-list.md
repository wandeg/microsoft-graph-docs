---
title: "List applications"
description: "List properties and relationships of the application objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List applications

Namespace: microsoft.graph

List properties and relationships of the [application](../resources/application.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /applications
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_application"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.application)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5543

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "275f3ac0-3ac0-275f-c03a-5f27c03a5f27",
      "deletedDateTime": "2017-01-01T00:02:42.9789072+03:00",
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn",
          "id": "438e8956-8956-438e-5689-8e4356898e43",
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
          "d8c48f40-8f40-d8c4-408f-c4d8408fc4d8"
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
      "createdDateTime": "2017-01-01T00:02:24.618735+03:00",
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
          "endDateTime": "2016-12-31T23:57:11.7522995+03:00",
          "keyId": "b37b5c66-5c66-b37b-665c-7bb3665c7bb3",
          "startDateTime": "2016-12-31T23:59:14.2230899+03:00",
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
      "tokenEncryptionKeyId": "25b6c6cc-c6cc-25b6-ccc6-b625ccc6b625",
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
  ]
}
```

