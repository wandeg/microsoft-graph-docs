---
title: "windowsInformationProtectionPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsInformationProtectionPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [windowsInformationProtection](../resources/windowsinformationprotection.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/windowsinformationprotectionpolicy-assign.md)|None|**TODO: Add Description**|
|[List protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-list-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the protectedAppLockerFiles navigation property.|
|[Create protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-post-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Create a new protectedAppLockerFiles object.|
|[Delete protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-delete-protectedapplockerfiles.md)|None|Delete a [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[Update protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-update-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Update the properties of a protectedAppLockerFiles object.|
|[Get windowsInformationProtectionAppLockerFile](../api/windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Read the properties and relationships of a [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[List exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-list-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the exemptAppLockerFiles navigation property.|
|[Create exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-post-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Create a new exemptAppLockerFiles object.|
|[Delete exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-delete-exemptapplockerfiles.md)|None|Delete an [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[Update exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-update-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Update the properties of an exemptAppLockerFiles object.|
|[Get windowsInformationProtectionAppLockerFile](../api/windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Read the properties and relationships of a [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[List assignments](../api/windowsinformationprotectionpolicy-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/windowsinformationprotectionpolicy-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/windowsinformationprotectionpolicy-delete-assignments.md)|None|Delete an [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|
|[Update assignments](../api/windowsinformationprotectionpolicy-update-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Update the properties of an assignments object.|
|[Get targetedManagedAppPolicyAssignment](../api/targetedmanagedapppolicyassignment-get.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Read the properties and relationships of a [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureRightsManagementServicesAllowed|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/windowsinformationprotectiondatarecoverycertificate.md)|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|daysWithoutContactBeforeUnenroll|Int32|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|enforcementLevel|windowsInformationProtectionEnforcementLevel|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md). Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/windowsinformationprotectioniprangecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRangesAreAuthoritative|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/windowsinformationprotectionproxieddomaincollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServersAreAuthoritative|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|iconsVisible|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|indexingEncryptedStoresOrItemsBlocked|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|isAssigned|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|mdmEnrollmentUrl|String|**TODO: Add Description**|
|minutesOfInactivityBeforeDeviceLock|Int32|**TODO: Add Description**|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|numberOfPastPinsRemembered|Int32|**TODO: Add Description**|
|passwordMaximumAttemptCount|Int32|**TODO: Add Description**|
|pinExpirationDays|Int32|**TODO: Add Description**|
|pinLowercaseLetters|windowsInformationProtectionPinCharacterRequirements|**TODO: Add Description**. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinMinimumLength|Int32|**TODO: Add Description**|
|pinSpecialCharacters|windowsInformationProtectionPinCharacterRequirements|**TODO: Add Description**. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinUppercaseLetters|windowsInformationProtectionPinCharacterRequirements|**TODO: Add Description**. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|protectedApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectionUnderLockConfigRequired|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|revokeOnMdmHandoffDisabled|Boolean|**TODO: Add Description**|
|revokeOnUnenrollDisabled|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|rightsManagementServicesTemplateId|Guid|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|roleScopeTagIds|String collection|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|windowsHelloForBusinessBlocked|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionPolicy",
  "baseType": "microsoft.graph.windowsInformationProtection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "protectionUnderLockConfigRequired": "Boolean",
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
  },
  "revokeOnUnenrollDisabled": "Boolean",
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": "Boolean",
  "iconsVisible": "Boolean",
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
    }
  ],
  "enterpriseIPRangesAreAuthoritative": "Boolean",
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxyServersAreAuthoritative": "Boolean",
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": "Boolean",
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "isAssigned": "Boolean",
  "revokeOnMdmHandoffDisabled": "Boolean",
  "mdmEnrollmentUrl": "String",
  "windowsHelloForBusinessBlocked": "Boolean",
  "pinMinimumLength": "Integer",
  "pinUppercaseLetters": "String",
  "pinLowercaseLetters": "String",
  "pinSpecialCharacters": "String",
  "pinExpirationDays": "Integer",
  "numberOfPastPinsRemembered": "Integer",
  "passwordMaximumAttemptCount": "Integer",
  "minutesOfInactivityBeforeDeviceLock": "Integer",
  "daysWithoutContactBeforeUnenroll": "Integer"
}
```

