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
|[List windowsInformationProtectionPolicies](../api/intune-deviceappmanagement-list-windowsinformationprotectionpolicies.md)|[windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md) collection|Get the windowsInformationProtectionPolicies from the windowsInformationProtectionPolicies navigation property.|
|[Create windowsInformationProtectionPolicies](../api/intune-deviceappmanagement-post-windowsinformationprotectionpolicies.md)|[windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md)|Create a new windowsInformationProtectionPolicies object.|
|[Delete windowsInformationProtectionPolicies](../api/intune-deviceappmanagement-delete-windowsinformationprotectionpolicies.md)|None|Delete a [windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md) object.|
|[Update windowsInformationProtectionPolicies](../api/intune-deviceappmanagement-update-windowsinformationprotectionpolicies.md)|[windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md)|Update the properties of a windowsInformationProtectionPolicies object.|
|[Get windowsInformationProtectionPolicies](../api/intune-deviceappmanagement-get-windowsinformationprotectionpolicy.md)|[windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md)|Read the properties and relationships of a [windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md) object.|
|[assign](../api/windowsinformationprotectionpolicy-assign.md)|None|**TODO: Add Description**|
|[List protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-list-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the protectedAppLockerFiles navigation property.|
|[Create protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-post-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Create a new protectedAppLockerFiles object.|
|[Delete protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-delete-protectedapplockerfiles.md)|None|Delete a [windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) object.|
|[Update protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-update-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Update the properties of a protectedAppLockerFiles object.|
|[Get protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-get-windowsinformationprotectionapplockerfile.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Read the properties and relationships of a [windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) object.|
|[List exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-list-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the exemptAppLockerFiles navigation property.|
|[Create exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-post-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Create a new exemptAppLockerFiles object.|
|[Delete exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-delete-exemptapplockerfiles.md)|None|Delete a [windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) object.|
|[Update exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-update-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Update the properties of an exemptAppLockerFiles object.|
|[Get exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-get-windowsinformationprotectionapplockerfile.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Read the properties and relationships of a [windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) object.|
|[List assignments](../api/windowsinformationprotectionpolicy-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/windowsinformationprotectionpolicy-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/windowsinformationprotectionpolicy-delete-assignments.md)|None|Delete a [targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) object.|
|[Update assignments](../api/windowsinformationprotectionpolicy-update-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/windowsinformationprotectionpolicy-get-targetedmanagedapppolicyassignment.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Read the properties and relationships of a [targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureRightsManagementServicesAllowed|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune-windowsinformationprotectiondatarecoverycertificate.md)|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|daysWithoutContactBeforeUnenroll|Int32|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|enforcementLevel|windowsInformationProtectionEnforcementLevel|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md). Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/intune-windowsinformationprotectioniprangecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRangesAreAuthoritative|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/intune-windowsinformationprotectionproxieddomaincollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServersAreAuthoritative|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptApps|[windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|iconsVisible|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|indexingEncryptedStoresOrItemsBlocked|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|isAssigned|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|mdmEnrollmentUrl|String|**TODO: Add Description**|
|minutesOfInactivityBeforeDeviceLock|Int32|**TODO: Add Description**|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|numberOfPastPinsRemembered|Int32|**TODO: Add Description**|
|passwordMaximumAttemptCount|Int32|**TODO: Add Description**|
|pinExpirationDays|Int32|**TODO: Add Description**|
|pinLowercaseLetters|windowsInformationProtectionPinCharacterRequirements|**TODO: Add Description**. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinMinimumLength|Int32|**TODO: Add Description**|
|pinSpecialCharacters|windowsInformationProtectionPinCharacterRequirements|**TODO: Add Description**. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinUppercaseLetters|windowsInformationProtectionPinCharacterRequirements|**TODO: Add Description**. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|protectedApps|[windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectionUnderLockConfigRequired|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|revokeOnMdmHandoffDisabled|Boolean|**TODO: Add Description**|
|revokeOnUnenrollDisabled|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|rightsManagementServicesTemplateId|Guid|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|windowsHelloForBusinessBlocked|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|

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

