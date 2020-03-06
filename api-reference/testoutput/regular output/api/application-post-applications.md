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
|Header|Value|
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
|addIns|[addIn](../resources/addin.md) collection||
|api|[apiApplication](../resources/apiapplication.md)||
|appId|String||
|applicationTemplateId|String||
|appRoles|[appRole](../resources/approle.md) collection||
|isFallbackPublicClient|Boolean||
|identifierUris|String collection||
|createdDateTime|DateTimeOffset||
|publicClient|[publicClientApplication](../resources/publicclientapplication.md)||
|displayName|String||
|groupMembershipClaims|String||
|info|[informationalUrl](../resources/informationalurl.md)||
|isDeviceOnlyAuthSupported|Boolean||
|keyCredentials|[keyCredential](../resources/keycredential.md) collection||
|logo|Stream||
|oauth2RequirePostResponse|Boolean||
|optionalClaims|[optionalClaims](../resources/optionalclaims.md)||
|parentalControlSettings|[parentalControlSettings](../resources/parentalcontrolsettings.md)||
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection||
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
POST https://graph.microsoft.com/localtest/applications
Content-type: application/json
Content-length: 4775

{
  "@odata.type": "#microsoft.graph.application",
  "deletedDateTime": "2016-12-31T23:59:54.5724597+03:00",
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "7fda8be5-8be5-7fda-e58b-da7fe58bda7f",
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
      "4b26af53-af53-4b26-53af-264b53af264b"
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
      "endDateTime": "2016-12-31T23:58:32.4599097+03:00",
      "keyId": "995554ed-54ed-9955-ed54-5599ed545599",
      "startDateTime": "2017-01-01T00:01:05.5047409+03:00",
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
  "tokenEncryptionKeyId": "51699f46-9f46-5169-469f-6951469f6951",
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
Content-Length: 4883

{
  "@odata.type": "#microsoft.graph.application",
  "id": "2cfed2c5-d2c5-2cfe-c5d2-fe2cc5d2fe2c",
  "deletedDateTime": "2016-12-31T23:59:54.5724597+03:00",
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "7fda8be5-8be5-7fda-e58b-da7fe58bda7f",
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
      "4b26af53-af53-4b26-53af-264b53af264b"
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
  "createdDateTime": "2016-12-31T23:57:43.7581228+03:00",
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
      "endDateTime": "2016-12-31T23:58:32.4599097+03:00",
      "keyId": "995554ed-54ed-9955-ed54-5599ed545599",
      "startDateTime": "2017-01-01T00:01:05.5047409+03:00",
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
  "tokenEncryptionKeyId": "51699f46-9f46-5169-469f-6951469f6951",
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
```

