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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /applications
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
If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.

## Examples

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
Content-Length: 5544

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "0f05fc37-fc37-0f05-37fc-050f37fc050f",
      "deletedDateTime": "2017-01-01T00:00:01.2462858+03:00",
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn",
          "id": "21c4e37a-e37a-21c4-7ae3-c4217ae3c421",
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
          "e2f4d82c-d82c-e2f4-2cd8-f4e22cd8f4e2"
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
      "createdDateTime": "2016-12-31T23:57:12.4657794+03:00",
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
          "endDateTime": "2016-12-31T23:57:14.1952433+03:00",
          "keyId": "bf2074b7-74b7-bf20-b774-20bfb77420bf",
          "startDateTime": "2016-12-31T23:56:36.5952464+03:00",
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
      "tokenEncryptionKeyId": "3b5a0ab2-0ab2-3b5a-b20a-5a3bb20a5a3b",
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

