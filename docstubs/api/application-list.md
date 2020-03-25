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
Content-Length: 5544

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "7ea836dd-36dd-7ea8-dd36-a87edd36a87e",
      "deletedDateTime": "2016-12-31T23:59:15.8984066+03:00",
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn",
          "id": "530adc71-dc71-530a-71dc-0a5371dc0a53",
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
          "8d8597d4-97d4-8d85-d497-858dd497858d"
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
      "createdDateTime": "2017-01-01T00:01:12.6625387+03:00",
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
          "endDateTime": "2016-12-31T23:56:48.6937674+03:00",
          "keyId": "1a94f160-f160-1a94-60f1-941a60f1941a",
          "startDateTime": "2017-01-01T00:01:40.4483143+03:00",
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
      "tokenEncryptionKeyId": "d9d51e51-1e51-d9d5-511e-d5d9511ed5d9",
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

