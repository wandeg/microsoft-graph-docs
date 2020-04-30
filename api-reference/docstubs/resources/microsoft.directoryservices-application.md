---
title: "application resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# application resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List applications](../api/microsoft.directoryservices-application-list.md)|[application](../resources/microsoft.directoryservices-application.md) collection|Get a list of the [application](../resources/application.md) objects and their properties.|
|[Get application](../api/microsoft.directoryservices-application-get.md)|[application](../resources/microsoft.directoryservices-application.md)|Read properties and relationships of an [application](../resources/microsoft.directoryservices-application.md) object.|
|[Create application](../api/microsoft.directoryservices-application-post-applications.md)|[application](../resources/microsoft.directoryservices-application.md)|Create a new [application](../resources/microsoft.directoryservices-application.md) object.|
|[Delete application](../api/microsoft.directoryservices-application-delete.md)|None|Deletes an [application](../resources/microsoft.directoryservices-application.md).|
|[Update application](../api/microsoft.directoryservices-application-update.md)|[application](../resources/microsoft.directoryservices-application.md)|Update the properties of a [application](../resources/microsoft.directoryservices-application.md) object.|
|[delta](../api/microsoft.directoryservices-application-delta.md)|[application](../resources/microsoft.directoryservices-application.md) collection|**TODO: Add Description**|
|[addKey](../api/microsoft.directoryservices-application-addkey.md)|[keyCredential](../resources/microsoft.directoryservices-keycredential.md)|**TODO: Add Description**|
|[addPassword](../api/microsoft.directoryservices-application-addpassword.md)|[passwordCredential](../resources/microsoft.directoryservices-passwordcredential.md)|**TODO: Add Description**|
|[checkMemberGroups](../api/microsoft.directoryservices-application-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-application-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-application-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-application-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-application-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[removeKey](../api/microsoft.directoryservices-application-removekey.md)|None|**TODO: Add Description**|
|[removePassword](../api/microsoft.directoryservices-application-removepassword.md)|None|**TODO: Add Description**|
|[List extensionProperties](../api/microsoft.directoryservices-application-list-extensionproperties.md)|[extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md) collection|Get the extensionProperties from the extensionProperties navigation property.|
|[Create extensionProperties](../api/microsoft.directoryservices-application-post-extensionproperties.md)|[extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md)|Create a new extensionProperties object.|
|[Delete extensionProperties](../api/microsoft.directoryservices-application-delete-extensionproperties.md)|None|Delete an extensionProperties object.|
|[Update extensionProperties](../api/microsoft.directoryservices-application-update-extensionproperties.md)|[extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md)|Update the properties of an extensionProperties object.|
|[Get extensionProperty](../api/microsoft.directoryservices-extensionproperty-get.md)|[extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md)|Read properties and relationships of an [extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md) object.|
|[List createdOnBehalfOf](../api/microsoft.directoryservices-application-list-createdonbehalfof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the createdOnBehalfOf navigation property.|
|[Add createdOnBehalfOf](../api/microsoft.directoryservices-application-post-createdonbehalfof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add createdOnBehalfOf by posting to the createdOnBehalfOf collection.|
|[Remove createdOnBehalfOf](../api/microsoft.directoryservices-application-delete-createdonbehalfof.md)|None|Remove a createdOnBehalfOf object.|
|[List owners](../api/microsoft.directoryservices-application-list-owners.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Add owners](../api/microsoft.directoryservices-application-post-owners.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add owners by posting to the owners collection.|
|[Remove owners](../api/microsoft.directoryservices-application-delete-owners.md)|None|Remove an owners object.|
|[List homeRealmDiscoveryPolicies](../api/microsoft.directoryservices-application-list-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md) collection|Get the homeRealmDiscoveryPolicies from the homeRealmDiscoveryPolicies navigation property.|
|[Add homeRealmDiscoveryPolicies](../api/microsoft.directoryservices-application-post-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md)|Add homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection.|
|[Remove homeRealmDiscoveryPolicies](../api/microsoft.directoryservices-application-delete-homerealmdiscoverypolicies.md)|None|Remove a homeRealmDiscoveryPolicies object.|
|[List policies](../api/microsoft.directoryservices-application-list-policies.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the policies navigation property.|
|[Add policies](../api/microsoft.directoryservices-application-post-policies.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add policies by posting to the policies collection.|
|[Remove policies](../api/microsoft.directoryservices-application-delete-policies.md)|None|Remove a policies object.|
|[List tokenIssuancePolicies](../api/microsoft.directoryservices-application-list-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/microsoft.directoryservices-tokenissuancepolicy.md) collection|Get the tokenIssuancePolicies from the tokenIssuancePolicies navigation property.|
|[Add tokenIssuancePolicies](../api/microsoft.directoryservices-application-post-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/microsoft.directoryservices-tokenissuancepolicy.md)|Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection.|
|[Remove tokenIssuancePolicies](../api/microsoft.directoryservices-application-delete-tokenissuancepolicies.md)|None|Remove a tokenIssuancePolicies object.|
|[List tokenLifetimePolicies](../api/microsoft.directoryservices-application-list-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/microsoft.directoryservices-tokenlifetimepolicy.md) collection|Get the tokenLifetimePolicies from the tokenLifetimePolicies navigation property.|
|[Add tokenLifetimePolicies](../api/microsoft.directoryservices-application-post-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/microsoft.directoryservices-tokenlifetimepolicy.md)|Add tokenLifetimePolicies by posting to the tokenLifetimePolicies collection.|
|[Remove tokenLifetimePolicies](../api/microsoft.directoryservices-application-delete-tokenlifetimepolicies.md)|None|Remove a tokenLifetimePolicies object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|api|[apiApplication](../resources/microsoft.directoryservices-apiapplication.md)|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|appRoles|[appRole](../resources/microsoft.directoryservices-approle.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|groupMembershipClaims|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|identifierUris|String collection|**TODO: Add Description**|
|info|[informationalUrl](../resources/microsoft.directoryservices-informationalurl.md)|**TODO: Add Description**|
|isDeviceOnlyAuthSupported|Boolean|**TODO: Add Description**|
|isFallbackPublicClient|Boolean|**TODO: Add Description**|
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

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdOnBehalfOf|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|extensionProperties|[extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md) collection|**TODO: Add Description**|
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](../resources/microsoft.directoryservices-homerealmdiscoverypolicy.md) collection|**TODO: Add Description**|
|owners|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|policies|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|tokenIssuancePolicies|[tokenIssuancePolicy](../resources/microsoft.directoryservices-tokenissuancepolicy.md) collection|**TODO: Add Description**|
|tokenLifetimePolicies|[tokenLifetimePolicy](../resources/microsoft.directoryservices-tokenlifetimepolicy.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.application",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.application",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "api": {
    "@odata.type": "Microsoft.DirectoryServices.apiApplication",
    "acceptMappedClaims": true,
    "knownClientApplications": [
      "Guid"
    ],
    "preAuthorizedApplications": [
      {
        "@odata.type": "Microsoft.DirectoryServices.preAuthorizedApplication",
        "appId": "String",
        "permissionIds": [
          "String"
        ]
      }
    ],
    "requestedAccessTokenVersion": 1024,
    "oauth2PermissionScopes": [
      {
        "@odata.type": "Microsoft.DirectoryServices.permissionScope",
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
    ],
    "resourceSpecificApplicationPermissions": [
      {
        "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermission"
      }
    ]
  },
  "appId": "String",
  "appRoles": [
    {
      "@odata.type": "Microsoft.DirectoryServices.appRole",
      "allowedMemberTypes": [
        "String"
      ]
    }
  ],
  "createdDateTime": "String (timestamp)",
  "isFallbackPublicClient": true,
  "identifierUris": [
    "String"
  ],
  "groupMembershipClaims": 1024,
  "info": {
    "@odata.type": "Microsoft.DirectoryServices.informationalUrl",
    "logoUrl": "String",
    "marketingUrl": "String",
    "privacyStatementUrl": "String",
    "supportUrl": "String",
    "termsOfServiceUrl": "String"
  },
  "isDeviceOnlyAuthSupported": true,
  "keyCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.keyCredential",
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
    "@odata.type": "Microsoft.DirectoryServices.optionalClaims",
    "idToken": [
      {
        "@odata.type": "Microsoft.DirectoryServices.optionalClaim",
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
      "String"
    ],
    "legalAgeGroupRule": "String"
  },
  "passwordCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.passwordCredential",
      "secretText": "String",
      "hint": "String"
    }
  ],
  "publicClient": {
    "@odata.type": "Microsoft.DirectoryServices.publicClientApplication",
    "redirectUris": [
      "String"
    ]
  },
  "publisherDomain": "String",
  "requiredResourceAccess": [
    {
      "@odata.type": "Microsoft.DirectoryServices.requiredResourceAccess",
      "resourceAppId": "String",
      "resourceAccess": [
        {
          "@odata.type": "Microsoft.DirectoryServices.resourceAccess"
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
    "@odata.type": "Microsoft.DirectoryServices.webApplication",
    "homePageUrl": "String",
    "oauth2AllowImplicitFlow": true,
    "logoutUrl": "String",
    "implicitGrantSettings": {
      "@odata.type": "Microsoft.DirectoryServices.implicitGrantSettings",
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": true
    }
  }
}
```

