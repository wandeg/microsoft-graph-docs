---
title: "windowsInformationProtectionPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionPolicy resource type


Namespace: microsoft.graph




Inherits from [windowsInformationProtection](../resources/windowsinformationprotection.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionPolicy](../api/windowsinformationprotectionpolicy-get.md)|[windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md)|Read properties and relationships of the [windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md) object.|
|[Update windowsInformationProtectionPolicy](../api/windowsinformationprotectionpolicy-update.md)|[windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md)|Update the properties of a [windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md) object.|
|[assign](../api/windowsinformationprotectionpolicy-assign.md)|None||
|[List protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-list-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the protectedAppLockerFiles navigation property.|
|[Add protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-post-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Add protectedAppLockerFiles by posting to the protectedAppLockerFiles collection.|
|[List exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-list-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the exemptAppLockerFiles navigation property.|
|[Add exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-post-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Add exemptAppLockerFiles by posting to the exemptAppLockerFiles collection.|
|[List assignments](../api/windowsinformationprotectionpolicy-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsinformationprotectionpolicy-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureRightsManagementServicesAllowed|Boolean| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|createdDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/windowsinformationprotectiondatarecoverycertificate.md)| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|daysWithoutContactBeforeUnenroll|Int32||
|description|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|displayName|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|enforcementLevel|Enumeration| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md). Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/windowsinformationprotectioniprangecollection.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRangesAreAuthoritative|Boolean| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/windowsinformationprotectionproxieddomaincollection.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServersAreAuthoritative|Boolean| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|iconsVisible|Boolean| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|indexingEncryptedStoresOrItemsBlocked|Boolean| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|isAssigned|Boolean| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|mdmEnrollmentUrl|String||
|minutesOfInactivityBeforeDeviceLock|Int32||
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|numberOfPastPinsRemembered|Int32||
|passwordMaximumAttemptCount|Int32||
|pinExpirationDays|Int32||
|pinLowercaseLetters|Enumeration| Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinMinimumLength|Int32||
|pinSpecialCharacters|Enumeration| Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinUppercaseLetters|Enumeration| Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|protectedApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectionUnderLockConfigRequired|Boolean| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|revokeOnMdmHandoffDisabled|Boolean||
|revokeOnUnenrollDisabled|Boolean| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|rightsManagementServicesTemplateId|Guid| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|roleScopeTagIds|String collection| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|version|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|windowsHelloForBusinessBlocked|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection| Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|

## JSON representation
Here is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "publisherName": "String",
      "productName": "String",
      "denied": true
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
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv4CidrRange",
          "cidrAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
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
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "String",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 1024,
  "pinUppercaseLetters": "String",
  "pinLowercaseLetters": "String",
  "pinSpecialCharacters": "String",
  "pinExpirationDays": 1024,
  "numberOfPastPinsRemembered": 1024,
  "passwordMaximumAttemptCount": 1024,
  "minutesOfInactivityBeforeDeviceLock": 1024,
  "daysWithoutContactBeforeUnenroll": 1024
}
```

