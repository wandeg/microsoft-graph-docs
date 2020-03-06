---
title: "applicationServicePrincipal resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# applicationServicePrincipal resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|application|[application](../resources/application.md)||
|servicePrincipal|[servicePrincipal](../resources/serviceprincipal.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applicationServicePrincipal",
  "application": {
    "@odata.type": "#microsoft.graph.application",
    "id": "String (identifier)",
    "deletedDateTime": "String (timestamp)",
    "api": {
      "@odata.type": "microsoft.graph.apiApplication",
      "acceptMappedClaims": true,
      "knownClientApplications": [
        "Guid"
      ],
      "preAuthorizedApplications": [
        {
          "@odata.type": "microsoft.graph.preAuthorizedApplication",
          "appId": "String",
          "permissionIds": [
            "String"
          ]
        }
      ],
      "requestedAccessTokenVersion": 1024,
      "oauth2PermissionScopes": [
        {
          "@odata.type": "microsoft.graph.permissionScope",
          "adminConsentDescription": "String",
          "adminConsentDisplayName": "String",
          "id": "Guid",
          "isEnabled": true,
          "origin": "String",
          "type": "String",
          "userConsentDescription": "String",
          "userConsentDisplayName": "String",
          "value": "String"
        }
      ]
    },
    "appId": "String",
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole",
        "allowedMemberTypes": [
          "String"
        ],
        "description": "String",
        "displayName": "String"
      }
    ],
    "createdDateTime": "String (timestamp)",
    "isFallbackPublicClient": true,
    "identifierUris": [
      "String"
    ],
    "displayName": "String",
    "groupMembershipClaims": "String",
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl",
      "logoUrl": "String",
      "marketingUrl": "String",
      "privacyStatementUrl": "String",
      "supportUrl": "String",
      "termsOfServiceUrl": "String"
    },
    "isDeviceOnlyAuthSupported": true,
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential",
        "customKeyIdentifier": "binary",
        "endDateTime": "String (timestamp)",
        "keyId": "Guid",
        "startDateTime": "String (timestamp)",
        "usage": "String",
        "key": "binary"
      }
    ],
    "logo": "Stream",
    "optionalClaims": {
      "@odata.type": "microsoft.graph.optionalClaims",
      "idToken": [
        {
          "@odata.type": "microsoft.graph.optionalClaim",
          "name": "String",
          "source": "String",
          "essential": true,
          "additionalProperties": [
            "String"
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
        "String"
      ],
      "legalAgeGroupRule": "String"
    },
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential",
        "secretText": "String",
        "hint": "String"
      }
    ],
    "publicClient": {
      "@odata.type": "microsoft.graph.publicClientApplication",
      "redirectUris": [
        "String"
      ]
    },
    "publisherDomain": "String",
    "requiredResourceAccess": [
      {
        "@odata.type": "microsoft.graph.requiredResourceAccess",
        "resourceAppId": "String",
        "resourceAccess": [
          {
            "@odata.type": "microsoft.graph.resourceAccess"
          }
        ]
      }
    ],
    "signInAudience": "String",
    "tags": [
      "String"
    ],
    "tokenEncryptionKeyId": "Guid",
    "web": {
      "@odata.type": "microsoft.graph.webApplication",
      "homePageUrl": "String",
      "oauth2AllowImplicitFlow": true,
      "logoutUrl": "String",
      "implicitGrantSettings": {
        "@odata.type": "microsoft.graph.implicitGrantSettings",
        "enableIdTokenIssuance": true,
        "enableAccessTokenIssuance": true
      }
    }
  },
  "servicePrincipal": {
    "@odata.type": "#microsoft.graph.servicePrincipal",
    "id": "String (identifier)",
    "deletedDateTime": "String (timestamp)",
    "accountEnabled": true,
    "addIns": [
      {
        "@odata.type": "microsoft.graph.addIn",
        "properties": [
          {
            "@odata.type": "microsoft.graph.keyValue",
            "key": "String"
          }
        ]
      }
    ],
    "appDisplayName": "String",
    "appId": "String",
    "applicationTemplateId": "String",
    "appOwnerOrganizationId": "Guid",
    "appRoleAssignmentRequired": true,
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole"
      }
    ],
    "displayName": "String",
    "homepage": "String",
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential"
      }
    ],
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl"
    },
    "logoutUrl": "String",
    "notificationEmailAddresses": [
      "String"
    ],
    "publishedPermissionScopes": [
      {
        "@odata.type": "microsoft.graph.permissionScope"
      }
    ],
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential"
      }
    ],
    "preferredTokenSigningKeyThumbprint": "String",
    "publisherName": "String",
    "replyUrls": [
      "String"
    ],
    "samlMetadataUrl": "String",
    "servicePrincipalNames": [
      "String"
    ],
    "tags": [
      "String"
    ]
  }
}
```

