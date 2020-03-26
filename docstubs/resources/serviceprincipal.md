---
title: "servicePrincipal resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# servicePrincipal resource type


Namespace: microsoft.graph




Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List servicePrincipals](../api/serviceprincipal-list.md)|[servicePrincipal](../resources/serviceprincipal.md) collection|List properties and relationships of the [servicePrincipal](../resources/serviceprincipal.md) objects.|
|[Get servicePrincipal](../api/serviceprincipal-get.md)|[servicePrincipal](../resources/serviceprincipal.md)|Read properties and relationships of the [servicePrincipal](../resources/serviceprincipal.md) object.|
|[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)|[servicePrincipal](../resources/serviceprincipal.md)|Create a new [servicePrincipal](../resources/serviceprincipal.md) object.|
|[Delete servicePrincipal](../api/serviceprincipal-delete.md)|None|Deletes a [servicePrincipal](../resources/serviceprincipal.md).|
|[Update servicePrincipal](../api/serviceprincipal-update.md)|[servicePrincipal](../resources/serviceprincipal.md)|Update the properties of a [servicePrincipal](../resources/serviceprincipal.md) object.|
|[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md)||
|[getPasswordSingleSignOnCredentials](../api/serviceprincipal-getpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md)||
|[deletePasswordSingleSignOnCredentials](../api/serviceprincipal-deletepasswordsinglesignoncredentials.md)|None||
|[updatePasswordSingleSignOnCredentials](../api/serviceprincipal-updatepasswordsinglesignoncredentials.md)|None||
|[delta](../api/serviceprincipal-delta.md)|[servicePrincipal](../resources/serviceprincipal.md) collection||
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String collection||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String collection||
|[restore](../api/serviceprincipal-restore.md)|[directoryObject](../resources/directoryobject.md)||
|[List appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md)|[appRoleAssignment](../resources/approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignedTo navigation property.|
|[Add appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md)|[appRoleAssignment](../resources/approleassignment.md)|Add appRoleAssignedTo by posting to the appRoleAssignedTo collection.|
|[List appRoleAssignments](../api/serviceprincipal-list-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Add appRoleAssignments](../api/serviceprincipal-post-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Add appRoleAssignments by posting to the appRoleAssignments collection.|
|[List claimsMappingPolicies](../api/serviceprincipal-list-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|Get the claimsMappingPolicies from the claimsMappingPolicies navigation property.|
|[Create claimsMappingPolicies](../api/serviceprincipal-post-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Create claimsMappingPolicies by posting to the claimsMappingPolicies collection.|
|[List homeRealmDiscoveryPolicies](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|Get the homeRealmDiscoveryPolicies from the homeRealmDiscoveryPolicies navigation property.|
|[Create homeRealmDiscoveryPolicies](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Create homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection.|
|[List endpoints](../api/serviceprincipal-list-endpoints.md)|[endpoint](../resources/endpoint.md) collection|Get the endpoints from the endpoints navigation property.|
|[Add endpoints](../api/serviceprincipal-post-endpoints.md)|[endpoint](../resources/endpoint.md)|Add endpoints by posting to the endpoints collection.|
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|Get the oAuth2PermissionGrants from the oauth2PermissionGrants navigation property.|
|[Create oauth2PermissionGrants](../api/serviceprincipal-post-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)|Create oauth2PermissionGrants by posting to the oauth2PermissionGrants collection.|
|[List memberOf](../api/serviceprincipal-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Create memberOf](../api/serviceprincipal-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Create memberOf by posting to the memberOf collection.|
|[List transitiveMemberOf](../api/serviceprincipal-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Create transitiveMemberOf](../api/serviceprincipal-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Create transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the createdObjects navigation property.|
|[Create createdObjects](../api/serviceprincipal-post-createdobjects.md)|[directoryObject](../resources/directoryobject.md)|Create createdObjects by posting to the createdObjects collection.|
|[List licenseDetails](../api/serviceprincipal-list-licensedetails.md)|[licenseDetails](../resources/licensedetails.md) collection|Get the licenseDetailses from the licenseDetails navigation property.|
|[Add licenseDetails](../api/serviceprincipal-post-licensedetails.md)|[licenseDetails](../resources/licensedetails.md)|Add licenseDetails by posting to the licenseDetails collection.|
|[List owners](../api/serviceprincipal-list-owners.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Create owners](../api/serviceprincipal-post-owners.md)|[directoryObject](../resources/directoryobject.md)|Create owners by posting to the owners collection.|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the ownedObjects navigation property.|
|[Create ownedObjects](../api/serviceprincipal-post-ownedobjects.md)|[directoryObject](../resources/directoryobject.md)|Create ownedObjects by posting to the ownedObjects collection.|
|[List tokenIssuancePolicies](../api/serviceprincipal-list-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|Get the tokenIssuancePolicies from the tokenIssuancePolicies navigation property.|
|[Create tokenIssuancePolicies](../api/serviceprincipal-post-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Create tokenIssuancePolicies by posting to the tokenIssuancePolicies collection.|
|[List tokenLifetimePolicies](../api/serviceprincipal-list-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|Get the tokenLifetimePolicies from the tokenLifetimePolicies navigation property.|
|[Create tokenLifetimePolicies](../api/serviceprincipal-post-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)|Create tokenLifetimePolicies by posting to the tokenLifetimePolicies collection.|
|[Get synchronization](../api/synchronization-get.md)|[synchronization](../resources/synchronization.md)|Read properties and relationships of the [synchronization](../resources/synchronization.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean||
|addIns|[addIn](../resources/addin.md) collection||
|alternativeNames|String collection||
|appDisplayName|String||
|appId|String||
|applicationTemplateId|String||
|appOwnerOrganizationId|Guid||
|appRoleAssignmentRequired|Boolean||
|appRoles|[appRole](../resources/approle.md) collection||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String||
|errorUrl|String||
|homepage|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|info|[informationalUrl](../resources/informationalurl.md)||
|keyCredentials|[keyCredential](../resources/keycredential.md) collection||
|loginUrl|String||
|logoutUrl|String||
|notificationEmailAddresses|String collection||
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection||
|preferredSingleSignOnMode|String||
|preferredTokenSigningKeyEndDateTime|DateTimeOffset||
|preferredTokenSigningKeyThumbprint|String||
|publishedPermissionScopes|[permissionScope](../resources/permissionscope.md) collection||
|publisherName|String||
|replyUrls|String collection||
|samlMetadataUrl|String||
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)||
|servicePrincipalNames|String collection||
|servicePrincipalType|String||
|signInAudience|String||
|tags|String collection||
|tokenEncryptionKeyId|Guid||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appRoleAssignedTo|[appRoleAssignment](../resources/approleassignment.md) collection||
|appRoleAssignments|[appRoleAssignment](../resources/approleassignment.md) collection||
|claimsMappingPolicies|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection||
|createdObjects|[directoryObject](../resources/directoryobject.md) collection||
|endpoints|[endpoint](../resources/endpoint.md) collection||
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection||
|licenseDetails|[licenseDetails](../resources/licensedetails.md) collection||
|memberOf|[directoryObject](../resources/directoryobject.md) collection||
|oauth2PermissionGrants|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection||
|ownedObjects|[directoryObject](../resources/directoryobject.md) collection||
|owners|[directoryObject](../resources/directoryobject.md) collection||
|synchronization|[synchronization](../resources/synchronization.md)||
|tokenIssuancePolicies|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection||
|tokenLifetimePolicies|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection||
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipal",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipal",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "Guid",
      "type": "String",
      "properties": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "String"
        }
      ]
    }
  ],
  "alternativeNames": [
    "String"
  ],
  "appDisplayName": "String",
  "appId": "String",
  "applicationTemplateId": "String",
  "appOwnerOrganizationId": "Guid",
  "appRoleAssignmentRequired": true,
  "appRoles": [
    {
      "@odata.type": "microsoft.graph.appRole",
      "allowedMemberTypes": [
        "String"
      ],
      "description": "String",
      "displayName": "String",
      "isEnabled": true,
      "origin": "String"
    }
  ],
  "displayName": "String",
  "errorUrl": "String",
  "homepage": "String",
  "info": {
    "@odata.type": "microsoft.graph.informationalUrl",
    "logoUrl": "String",
    "marketingUrl": "String",
    "privacyStatementUrl": "String",
    "supportUrl": "String",
    "termsOfServiceUrl": "String"
  },
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
  "loginUrl": "String",
  "logoutUrl": "String",
  "notificationEmailAddresses": [
    "String"
  ],
  "publishedPermissionScopes": [
    {
      "@odata.type": "microsoft.graph.permissionScope",
      "adminConsentDescription": "String",
      "adminConsentDisplayName": "String",
      "userConsentDescription": "String",
      "userConsentDisplayName": "String"
    }
  ],
  "passwordCredentials": [
    {
      "@odata.type": "microsoft.graph.passwordCredential",
      "secretText": "String",
      "hint": "String"
    }
  ],
  "preferredTokenSigningKeyEndDateTime": "String (timestamp)",
  "preferredTokenSigningKeyThumbprint": "String",
  "preferredSingleSignOnMode": "String",
  "publisherName": "String",
  "replyUrls": [
    "String"
  ],
  "samlMetadataUrl": "String",
  "samlSingleSignOnSettings": {
    "@odata.type": "microsoft.graph.samlSingleSignOnSettings",
    "relayState": "String"
  },
  "servicePrincipalNames": [
    "String"
  ],
  "servicePrincipalType": "String",
  "signInAudience": "String",
  "tags": [
    "String"
  ],
  "tokenEncryptionKeyId": "Guid"
}
```

