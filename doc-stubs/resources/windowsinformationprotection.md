---
title: "windowsInformationProtection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsInformationProtection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [managedAppPolicy](../resources/managedapppolicy.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/windowsinformationprotection-assign.md)|None|**TODO: Add Description**|
|[targetApps](../api/windowsinformationprotection-targetapps.md)|None|**TODO: Add Description**|
|[List protectedAppLockerFiles](../api/windowsinformationprotection-list-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the protectedAppLockerFiles navigation property.|
|[Create protectedAppLockerFiles](../api/windowsinformationprotection-post-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Create a new protectedAppLockerFiles object.|
|[Delete protectedAppLockerFiles](../api/windowsinformationprotection-delete-protectedapplockerfiles.md)|None|Delete a [windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) object.|
|[Update protectedAppLockerFiles](../api/windowsinformationprotection-update-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Update the properties of a protectedAppLockerFiles object.|
|[Get protectedAppLockerFiles](../api/windowsinformationprotection-get-windowsinformationprotectionapplockerfile.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Read the properties and relationships of a [windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) object.|
|[List exemptAppLockerFiles](../api/windowsinformationprotection-list-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the exemptAppLockerFiles navigation property.|
|[Create exemptAppLockerFiles](../api/windowsinformationprotection-post-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Create a new exemptAppLockerFiles object.|
|[Delete exemptAppLockerFiles](../api/windowsinformationprotection-delete-exemptapplockerfiles.md)|None|Delete a [windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) object.|
|[Update exemptAppLockerFiles](../api/windowsinformationprotection-update-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Update the properties of an exemptAppLockerFiles object.|
|[Get exemptAppLockerFiles](../api/windowsinformationprotection-get-windowsinformationprotectionapplockerfile.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md)|Read the properties and relationships of a [windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) object.|
|[List assignments](../api/windowsinformationprotection-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/windowsinformationprotection-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/windowsinformationprotection-delete-assignments.md)|None|Delete a [targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) object.|
|[Update assignments](../api/windowsinformationprotection-update-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Update the properties of an assignments object.|
|[Get assignments](../api/windowsinformationprotection-get-targetedmanagedapppolicyassignment.md)|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md)|Read the properties and relationships of a [targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureRightsManagementServicesAllowed|Boolean|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune-windowsinformationprotectiondatarecoverycertificate.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|enforcementLevel|windowsInformationProtectionEnforcementLevel|**TODO: Add Description**. Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String|**TODO: Add Description**|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description**|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/intune-windowsinformationprotectioniprangecollection.md) collection|**TODO: Add Description**|
|enterpriseIPRangesAreAuthoritative|Boolean|**TODO: Add Description**|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description**|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description**|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/intune-windowsinformationprotectionproxieddomaincollection.md) collection|**TODO: Add Description**|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description**|
|enterpriseProxyServersAreAuthoritative|Boolean|**TODO: Add Description**|
|exemptApps|[windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md) collection|**TODO: Add Description**|
|iconsVisible|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|indexingEncryptedStoresOrItemsBlocked|Boolean|**TODO: Add Description**|
|isAssigned|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description**|
|protectedApps|[windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md) collection|**TODO: Add Description**|
|protectionUnderLockConfigRequired|Boolean|**TODO: Add Description**|
|revokeOnUnenrollDisabled|Boolean|**TODO: Add Description**|
|rightsManagementServicesTemplateId|Guid|**TODO: Add Description**|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/intune-windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description**|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/intune-managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-targetedmanagedapppolicyassignment.md) collection|**TODO: Add Description**|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) collection|**TODO: Add Description**|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-windowsinformationprotectionapplockerfile.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection",
  "baseType": "microsoft.graph.managedAppPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
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
  "isAssigned": "Boolean"
}
```

