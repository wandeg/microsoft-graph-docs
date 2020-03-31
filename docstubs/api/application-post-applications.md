---
title: "Create application"
description: "Create a new application object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create application

Namespace: microsoft.graph

Create a new [application](../resources/application.md) object.

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
POST /applications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [application](../resources/application.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 4477

{
  "@odata.type": "#microsoft.graph.application",
  "deletedDateTime": "2016-12-31T23:58:43.3543606+03:00",
  "api": {
    "@odata.type": "microsoft.graph.apiApplication",
    "acceptMappedClaims": true,
    "knownClientApplications": [
      "0a6af7cd-f7cd-0a6a-cdf7-6a0acdf76a0a"
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
        "id": "24fb3ae4-3ae4-24fb-e43a-fb24e43afb24",
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
      "endDateTime": "2017-01-01T00:00:11.5602866+03:00",
      "keyId": "dac9645c-645c-dac9-5c64-c9da5c64c9da",
      "startDateTime": "2016-12-31T23:58:03.4514069+03:00",
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
  "tokenEncryptionKeyId": "df9b2c42-2c42-df9b-422c-9bdf422c9bdf",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4585

{
  "@odata.type": "#microsoft.graph.application",
  "id": "00c0d9cc-d9cc-00c0-ccd9-c000ccd9c000",
  "deletedDateTime": "2016-12-31T23:58:43.3543606+03:00",
  "api": {
    "@odata.type": "microsoft.graph.apiApplication",
    "acceptMappedClaims": true,
    "knownClientApplications": [
      "0a6af7cd-f7cd-0a6a-cdf7-6a0acdf76a0a"
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
        "id": "24fb3ae4-3ae4-24fb-e43a-fb24e43afb24",
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
  "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
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
      "endDateTime": "2017-01-01T00:00:11.5602866+03:00",
      "keyId": "dac9645c-645c-dac9-5c64-c9da5c64c9da",
      "startDateTime": "2016-12-31T23:58:03.4514069+03:00",
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
  "tokenEncryptionKeyId": "df9b2c42-2c42-df9b-422c-9bdf422c9bdf",
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

