---
title: "application resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# application resource type

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryObject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List applications](../api/application-list.md)|[application](../resources/application.md) collection|List properties and relationships of the [application](../resources/application.md) objects.|
|[Get application](../api/application-get.md)|[application](../resources/application.md)|Read properties and relationships of the [application](../resources/application.md) object.|
|[Create application](../api/application-post-applications.md)|[application](../resources/application.md)|Create a new [application](../resources/application.md) object.|
|[Delete application](../api/application-delete.md)|None|Deletes a [application](../resources/application.md).|
|[Update application](../api/application-update.md)|[application](../resources/application.md)|Update the properties of a [application](../resources/application.md) object.|
|[delta](../api/application-delta.md)|[application](../resources/application.md) collection||
|[addKey](../api/application-addkey.md)|[keyCredential](../resources/keyCredential.md)||
|[addPassword](../api/application-addpassword.md)|[passwordCredential](../resources/passwordCredential.md)||
|[removeKey](../api/application-removekey.md)|None||
|[removePassword](../api/application-removepassword.md)|None||
|[checkMemberGroups](../api/application-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/application-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/application-getmembergroups.md)|String collection||
|[getMemberObjects](../api/application-getmemberobjects.md)|String collection||
|[restore](../api/application-restore.md)|[directoryObject](../resources/directoryObject.md)||
|[List extensionProperties](../api/application-list-extensionproperties.md)|[extensionProperty](../resources/extensionProperty.md) collection|Get the extensionProperties from the extensionProperties navigation property.|
|[Add extensionProperties](../api/application-post-extensionproperties.md)|[extensionProperty](../resources/extensionProperty.md)|Add extensionProperties by posting to the extensionProperties collection.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryObject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[List owners](../api/application-list-owners.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Create owners](../api/application-post-owners.md)|[directoryObject](../resources/directoryObject.md)|Create owners by posting to the owners collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addIns|[addIn](../resources/addIn.md) collection||
|api|[apiApplication](../resources/apiApplication.md)||
|appId|String||
|applicationTemplateId|String||
|appRoles|[appRole](../resources/appRole.md) collection||
|createdDateTime|DateTimeOffset||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|displayName|String||
|groupMembershipClaims|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|identifierUris|String collection||
|info|[informationalUrl](../resources/informationalUrl.md)||
|isDeviceOnlyAuthSupported|Boolean||
|isFallbackPublicClient|Boolean||
|keyCredentials|[keyCredential](../resources/keyCredential.md) collection||
|logo|Stream||
|oauth2RequirePostResponse|Boolean||
|optionalClaims|[optionalClaims](../resources/optionalClaims.md)||
|parentalControlSettings|[parentalControlSettings](../resources/parentalControlSettings.md)||
|passwordCredentials|[passwordCredential](../resources/passwordCredential.md) collection||
|publicClient|[publicClientApplication](../resources/publicClientApplication.md)||
|publisherDomain|String||
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredResourceAccess.md) collection||
|signInAudience|String||
|tags|String collection||
|tokenEncryptionKeyId|Guid||
|web|[webApplication](../resources/webApplication.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdOnBehalfOf|[directoryObject](../resources/directoryObject.md)||
|extensionProperties|[extensionProperty](../resources/extensionProperty.md) collection||
|owners|[directoryObject](../resources/directoryObject.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.application",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.application",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "Guid",
      "type": "String",
      "properties": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "String",
          "value": "String"
        }
      ]
    }
  ],
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
        "delegatedPermissionIds": [
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
        "isEnabled": true,
        "origin": "String",
        "userConsentDescription": "String",
        "userConsentDisplayName": "String"
      }
    ]
  },
  "appId": "String",
  "applicationTemplateId": "String",
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
  "isFallbackPublicClient": true,
  "identifierUris": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "publicClient": {
    "@odata.type": "microsoft.graph.publicClientApplication",
    "redirectUris": [
      "String"
    ]
  },
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
  "oauth2RequirePostResponse": true,
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
    "logoutUrl": "String",
    "implicitGrantSettings": {
      "@odata.type": "microsoft.graph.implicitGrantSettings",
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": true
    }
  }
}
```

