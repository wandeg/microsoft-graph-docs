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
|Name|Description|
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
GET https://graph.microsoft.com/beta/applications
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
Content-Length: 5198

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "1451c400-c400-1451-00c4-511400c45114",
      "deletedDateTime": "2016-12-31T23:57:33.1327036+03:00",
      "api": {
        "@odata.type": "microsoft.graph.apiApplication",
        "acceptMappedClaims": true,
        "knownClientApplications": [
          "13d51127-1127-13d5-2711-d5132711d513"
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
            "id": "90b01f73-1f73-90b0-731f-b090731fb090",
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
      "createdDateTime": "2017-01-01T00:00:37.2865022+03:00",
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
          "endDateTime": "2016-12-31T23:59:11.8282448+03:00",
          "keyId": "af82b8a5-b8a5-af82-a5b8-82afa5b882af",
          "startDateTime": "2016-12-31T23:59:28.0884883+03:00",
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
      "tokenEncryptionKeyId": "0052e460-e460-0052-60e4-520060e45200",
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
  ]
}
```

