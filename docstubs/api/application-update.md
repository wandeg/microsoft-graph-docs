---
title: "Update application"
description: "Update the properties of a application object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update application

Namespace: microsoft.graph

Update the properties of a [application](../resources/application.md) object.

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
PATCH /applications/{applicationsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [application](../resources/application.md) object.

The following table shows the properties that are required when you create the [application](../resources/application.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|api|[apiApplication](../resources/apiapplication.md)||
|appId|String||
|appRoles|[appRole](../resources/approle.md) collection||
|createdDateTime|DateTimeOffset||
|isFallbackPublicClient|Boolean||
|identifierUris|String collection||
|displayName|String||
|groupMembershipClaims|String||
|info|[informationalUrl](../resources/informationalurl.md)||
|isDeviceOnlyAuthSupported|Boolean||
|keyCredentials|[keyCredential](../resources/keycredential.md) collection||
|logo|Stream||
|optionalClaims|[optionalClaims](../resources/optionalclaims.md)||
|parentalControlSettings|[parentalControlSettings](../resources/parentalcontrolsettings.md)||
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection||
|publicClient|[publicClientApplication](../resources/publicclientapplication.md)||
|publisherDomain|String||
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md) collection||
|signInAudience|String||
|tags|String collection||
|tokenEncryptionKeyId|Guid||
|web|[webApplication](../resources/webapplication.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [application](../resources/application.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_application"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}
Content-type: application/json
Content-length: 4477

{
  "@odata.type": "#microsoft.graph.application",
  "deletedDateTime": "2016-12-31T23:57:00.1067265+03:00",
  "api": {
    "@odata.type": "microsoft.graph.apiApplication",
    "acceptMappedClaims": true,
    "knownClientApplications": [
      "7af357a6-57a6-7af3-a657-f37aa657f37a"
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
        "id": "174827b3-27b3-1748-b327-4817b3274817",
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
      "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
      "keyId": "69850448-0448-6985-4804-856948048569",
      "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
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
  "tokenEncryptionKeyId": "db740ce5-0ce5-db74-e50c-74dbe50c74db",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4585

{
  "@odata.type": "#microsoft.graph.application",
  "id": "b258a24f-a24f-b258-4fa2-58b24fa258b2",
  "deletedDateTime": "2016-12-31T23:57:00.1067265+03:00",
  "api": {
    "@odata.type": "microsoft.graph.apiApplication",
    "acceptMappedClaims": true,
    "knownClientApplications": [
      "7af357a6-57a6-7af3-a657-f37aa657f37a"
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
        "id": "174827b3-27b3-1748-b327-4817b3274817",
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
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
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
      "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
      "keyId": "69850448-0448-6985-4804-856948048569",
      "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
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
  "tokenEncryptionKeyId": "db740ce5-0ce5-db74-e50c-74dbe50c74db",
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
```

