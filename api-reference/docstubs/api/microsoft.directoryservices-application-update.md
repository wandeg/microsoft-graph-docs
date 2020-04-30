---
title: "Update application"
description: "Update the properties of a application object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update application

Namespace: Microsoft.DirectoryServices

Update the properties of a [application](../resources/microsoft.directoryservices-application.md) object.

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
PATCH /applications/{applicationsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [application](../resources/microsoft.directoryservices-application.md) object.

The following table shows the properties that are required when you create the [application](../resources/microsoft.directoryservices-application.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|api|[apiApplication](../resources/microsoft.directoryservices-apiapplication.md)|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|appRoles|[appRole](../resources/microsoft.directoryservices-approle.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|isFallbackPublicClient|Boolean|**TODO: Add Description**|
|identifierUris|String collection|**TODO: Add Description**|
|groupMembershipClaims|Int32|**TODO: Add Description**|
|info|[informationalUrl](../resources/microsoft.directoryservices-informationalurl.md)|**TODO: Add Description**|
|isDeviceOnlyAuthSupported|Boolean|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/microsoft.directoryservices-keycredential.md) collection|**TODO: Add Description**|
|logo|Stream|**TODO: Add Description**|
|optionalClaims|[optionalClaims](../resources/microsoft.directoryservices-optionalclaims.md)|**TODO: Add Description**|
|parentalControlSettings|[parentalControlSettings](../resources/microsoft.directoryservices-parentalcontrolsettings.md)|**TODO: Add Description**|
|passwordCredentials|[passwordCredential](../resources/microsoft.directoryservices-passwordcredential.md) collection|**TODO: Add Description**|
|publicClient|[publicClientApplication](../resources/microsoft.directoryservices-publicclientapplication.md)|**TODO: Add Description**|
|publisherDomain|String|**TODO: Add Description**|
|requiredResourceAccess|[requiredResourceAccess](../resources/microsoft.directoryservices-requiredresourceaccess.md) collection|**TODO: Add Description**|
|signInAudience|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|tokenEncryptionKeyId|Guid|**TODO: Add Description**|
|web|[webApplication](../resources/microsoft.directoryservices-webapplication.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [application](../resources/microsoft.directoryservices-application.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_application"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/applications/{applicationsId}
Content-Type: application/json
Content-length: 4783

{
  "@odata.type": "#Microsoft.DirectoryServices.application",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "api": {
    "@odata.type": "Microsoft.DirectoryServices.apiApplication",
    "acceptMappedClaims": true,
    "knownClientApplications": [
      "ed7ed1e9-d1e9-ed7e-e9d1-7eede9d17eed"
    ],
    "preAuthorizedApplications": [
      {
        "@odata.type": "Microsoft.DirectoryServices.preAuthorizedApplication",
        "appId": "App Id value",
        "permissionIds": [
          "Permission Ids value"
        ]
      }
    ],
    "requestedAccessTokenVersion": 11,
    "oauth2PermissionScopes": [
      {
        "@odata.type": "Microsoft.DirectoryServices.permissionScope",
        "adminConsentDescription": "Admin Consent Description value",
        "adminConsentDisplayName": "Admin Consent Display Name value",
        "id": "6ce1b2dc-b2dc-6ce1-dcb2-e16cdcb2e16c",
        "isEnabled": true,
        "origin": "Origin value",
        "type": "Type value",
        "userConsentDescription": "User Consent Description value",
        "userConsentDisplayName": "User Consent Display Name value",
        "value": "Value value"
      }
    ],
    "resourceSpecificApplicationPermissions": [
      {
        "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermission",
        "description": "Description value",
        "displayName": "Display Name value"
      }
    ]
  },
  "appId": "App Id value",
  "appRoles": [
    {
      "@odata.type": "Microsoft.DirectoryServices.appRole",
      "allowedMemberTypes": [
        "Allowed Member Types value"
      ]
    }
  ],
  "isFallbackPublicClient": true,
  "identifierUris": [
    "Identifier Uris value"
  ],
  "groupMembershipClaims": 5,
  "info": {
    "@odata.type": "Microsoft.DirectoryServices.informationalUrl",
    "logoUrl": "https://example.com/logoUrl/",
    "marketingUrl": "https://example.com/marketingUrl/",
    "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
    "supportUrl": "https://example.com/supportUrl/",
    "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
  },
  "isDeviceOnlyAuthSupported": true,
  "keyCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.keyCredential",
      "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
      "endDateTime": "2017-01-01T00:01:58.2456509+00:00",
      "keyId": "c4860b27-0b27-c486-270b-86c4270b86c4",
      "startDateTime": "2017-01-01T00:01:26.5340071+00:00",
      "usage": "Usage value",
      "key": "a2V5"
    }
  ],
  "logo": "Stream",
  "optionalClaims": {
    "@odata.type": "Microsoft.DirectoryServices.optionalClaims",
    "idToken": [
      {
        "@odata.type": "Microsoft.DirectoryServices.optionalClaim",
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
        "@odata.type": "Microsoft.DirectoryServices.optionalClaim"
      }
    ],
    "saml2Token": [
      {
        "@odata.type": "Microsoft.DirectoryServices.optionalClaim"
      }
    ]
  },
  "parentalControlSettings": {
    "@odata.type": "Microsoft.DirectoryServices.parentalControlSettings",
    "countriesBlockedForMinors": [
      "Countries Blocked For Minors value"
    ],
    "legalAgeGroupRule": "Legal Age Group Rule value"
  },
  "passwordCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.passwordCredential",
      "secretText": "Secret Text value",
      "hint": "Hint value"
    }
  ],
  "publicClient": {
    "@odata.type": "Microsoft.DirectoryServices.publicClientApplication",
    "redirectUris": [
      "Redirect Uris value"
    ]
  },
  "publisherDomain": "Publisher Domain value",
  "requiredResourceAccess": [
    {
      "@odata.type": "Microsoft.DirectoryServices.requiredResourceAccess",
      "resourceAppId": "Resource App Id value",
      "resourceAccess": [
        {
          "@odata.type": "Microsoft.DirectoryServices.resourceAccess"
        }
      ]
    }
  ],
  "signInAudience": "Sign In Audience value",
  "tags": [
    "Tags value"
  ],
  "tokenEncryptionKeyId": "992a9363-9363-992a-6393-2a9963932a99",
  "web": {
    "@odata.type": "Microsoft.DirectoryServices.webApplication",
    "homePageUrl": "https://example.com/homePageUrl/",
    "oauth2AllowImplicitFlow": true,
    "logoutUrl": "https://example.com/logoutUrl/",
    "implicitGrantSettings": {
      "@odata.type": "Microsoft.DirectoryServices.implicitGrantSettings",
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": true
    }
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.application",
  "id": "9ce4c367-c367-9ce4-67c3-e49c67c3e49c",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "api": {
    "@odata.type": "Microsoft.DirectoryServices.apiApplication",
    "acceptMappedClaims": true,
    "knownClientApplications": [
      "ed7ed1e9-d1e9-ed7e-e9d1-7eede9d17eed"
    ],
    "preAuthorizedApplications": [
      {
        "@odata.type": "Microsoft.DirectoryServices.preAuthorizedApplication",
        "appId": "App Id value",
        "permissionIds": [
          "Permission Ids value"
        ]
      }
    ],
    "requestedAccessTokenVersion": 11,
    "oauth2PermissionScopes": [
      {
        "@odata.type": "Microsoft.DirectoryServices.permissionScope",
        "adminConsentDescription": "Admin Consent Description value",
        "adminConsentDisplayName": "Admin Consent Display Name value",
        "id": "6ce1b2dc-b2dc-6ce1-dcb2-e16cdcb2e16c",
        "isEnabled": true,
        "origin": "Origin value",
        "type": "Type value",
        "userConsentDescription": "User Consent Description value",
        "userConsentDisplayName": "User Consent Display Name value",
        "value": "Value value"
      }
    ],
    "resourceSpecificApplicationPermissions": [
      {
        "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermission",
        "description": "Description value",
        "displayName": "Display Name value"
      }
    ]
  },
  "appId": "App Id value",
  "appRoles": [
    {
      "@odata.type": "Microsoft.DirectoryServices.appRole",
      "allowedMemberTypes": [
        "Allowed Member Types value"
      ]
    }
  ],
  "createdDateTime": "2017-01-01T00:03:17.7218452+00:00",
  "isFallbackPublicClient": true,
  "identifierUris": [
    "Identifier Uris value"
  ],
  "groupMembershipClaims": 5,
  "info": {
    "@odata.type": "Microsoft.DirectoryServices.informationalUrl",
    "logoUrl": "https://example.com/logoUrl/",
    "marketingUrl": "https://example.com/marketingUrl/",
    "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
    "supportUrl": "https://example.com/supportUrl/",
    "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
  },
  "isDeviceOnlyAuthSupported": true,
  "keyCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.keyCredential",
      "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
      "endDateTime": "2017-01-01T00:01:58.2456509+00:00",
      "keyId": "c4860b27-0b27-c486-270b-86c4270b86c4",
      "startDateTime": "2017-01-01T00:01:26.5340071+00:00",
      "usage": "Usage value",
      "key": "a2V5"
    }
  ],
  "logo": "Stream",
  "optionalClaims": {
    "@odata.type": "Microsoft.DirectoryServices.optionalClaims",
    "idToken": [
      {
        "@odata.type": "Microsoft.DirectoryServices.optionalClaim",
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
        "@odata.type": "Microsoft.DirectoryServices.optionalClaim"
      }
    ],
    "saml2Token": [
      {
        "@odata.type": "Microsoft.DirectoryServices.optionalClaim"
      }
    ]
  },
  "parentalControlSettings": {
    "@odata.type": "Microsoft.DirectoryServices.parentalControlSettings",
    "countriesBlockedForMinors": [
      "Countries Blocked For Minors value"
    ],
    "legalAgeGroupRule": "Legal Age Group Rule value"
  },
  "passwordCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.passwordCredential",
      "secretText": "Secret Text value",
      "hint": "Hint value"
    }
  ],
  "publicClient": {
    "@odata.type": "Microsoft.DirectoryServices.publicClientApplication",
    "redirectUris": [
      "Redirect Uris value"
    ]
  },
  "publisherDomain": "Publisher Domain value",
  "requiredResourceAccess": [
    {
      "@odata.type": "Microsoft.DirectoryServices.requiredResourceAccess",
      "resourceAppId": "Resource App Id value",
      "resourceAccess": [
        {
          "@odata.type": "Microsoft.DirectoryServices.resourceAccess"
        }
      ]
    }
  ],
  "signInAudience": "Sign In Audience value",
  "tags": [
    "Tags value"
  ],
  "tokenEncryptionKeyId": "992a9363-9363-992a-6393-2a9963932a99",
  "web": {
    "@odata.type": "Microsoft.DirectoryServices.webApplication",
    "homePageUrl": "https://example.com/homePageUrl/",
    "oauth2AllowImplicitFlow": true,
    "logoutUrl": "https://example.com/logoutUrl/",
    "implicitGrantSettings": {
      "@odata.type": "Microsoft.DirectoryServices.implicitGrantSettings",
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": true
    }
  }
}
```

