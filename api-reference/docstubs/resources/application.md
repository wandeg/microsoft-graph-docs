---
title: "application resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# application resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List applications](../api/application-list.md)|[application](../resources/application.md) collection|Get a list of the [application](../resources/application.md) objects and their properties.|
|[Get application](../api/application-get.md)|[application](../resources/application.md)|Read properties and relationships of an [application](../resources/application.md) object.|
|[Create application](../api/application-post-applications.md)|[application](../resources/application.md)|Create a new [application](../resources/application.md) object.|
|[Delete application](../api/application-delete.md)|None|Deletes an [application](../resources/application.md).|
|[Update application](../api/application-update.md)|[application](../resources/application.md)|Update the properties of a [application](../resources/application.md) object.|
|[delta](../api/application-delta.md)|[application](../resources/application.md) collection|**TODO: Add Description**|
|[addKey](../api/application-addkey.md)|[keyCredential](../resources/keycredential.md)|**TODO: Add Description**|
|[addPassword](../api/application-addpassword.md)|[passwordCredential](../resources/passwordcredential.md)|**TODO: Add Description**|
|[removeKey](../api/application-removekey.md)|None|**TODO: Add Description**|
|[removePassword](../api/application-removepassword.md)|None|**TODO: Add Description**|
|[checkMemberGroups](../api/application-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/application-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/application-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/application-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/application-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[List extensionProperties](../api/application-list-extensionproperties.md)|[extensionProperty](../resources/extensionproperty.md) collection|Get the extensionProperties from the extensionProperties navigation property.|
|[Create extensionProperties](../api/application-post-extensionproperties.md)|[extensionProperty](../resources/extensionproperty.md)|Create a new extensionProperties object.|
|[Delete extensionProperties](../api/application-delete-extensionproperties.md)|None|Delete an extensionProperties object.|
|[Update extensionProperties](../api/application-update-extensionproperties.md)|[extensionProperty](../resources/extensionproperty.md)|Update the properties of an extensionProperties object.|
|[Get extensionProperty](../api/extensionproperty-get.md)|[extensionProperty](../resources/extensionproperty.md)|Read properties and relationships of an [extensionProperty](../resources/extensionproperty.md) object.|
|[List createdOnBehalfOf](../api/application-list-createdonbehalfof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the createdOnBehalfOf navigation property.|
|[Add createdOnBehalfOf](../api/application-post-createdonbehalfof.md)|[directoryObject](../resources/directoryobject.md)|Add createdOnBehalfOf by posting to the createdOnBehalfOf collection.|
|[Remove createdOnBehalfOf](../api/application-delete-createdonbehalfof.md)|None|Remove a createdOnBehalfOf object.|
|[List owners](../api/application-list-owners.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Add owners](../api/application-post-owners.md)|[directoryObject](../resources/directoryobject.md)|Add owners by posting to the owners collection.|
|[Remove owners](../api/application-delete-owners.md)|None|Remove an owners object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addIns|[addIn](../resources/addin.md) collection|**TODO: Add Description**|
|api|[apiApplication](../resources/apiapplication.md)|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|applicationTemplateId|String|**TODO: Add Description**|
|appRoles|[appRole](../resources/approle.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|groupMembershipClaims|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|identifierUris|String collection|**TODO: Add Description**|
|info|[informationalUrl](../resources/informationalurl.md)|**TODO: Add Description**|
|isDeviceOnlyAuthSupported|Boolean|**TODO: Add Description**|
|isFallbackPublicClient|Boolean|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|**TODO: Add Description**|
|logo|Stream|**TODO: Add Description**|
|oauth2RequirePostResponse|Boolean|**TODO: Add Description**|
|optionalClaims|[optionalClaims](../resources/optionalclaims.md)|**TODO: Add Description**|
|parentalControlSettings|[parentalControlSettings](../resources/parentalcontrolsettings.md)|**TODO: Add Description**|
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection|**TODO: Add Description**|
|publicClient|[publicClientApplication](../resources/publicclientapplication.md)|**TODO: Add Description**|
|publisherDomain|String|**TODO: Add Description**|
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md) collection|**TODO: Add Description**|
|signInAudience|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|tokenEncryptionKeyId|Guid|**TODO: Add Description**|
|web|[webApplication](../resources/webapplication.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdOnBehalfOf|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|extensionProperties|[extensionProperty](../resources/extensionproperty.md) collection|**TODO: Add Description**|
|owners|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
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

