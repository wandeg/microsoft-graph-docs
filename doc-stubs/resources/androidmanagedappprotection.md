---
title: "androidManagedAppProtection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidManagedAppProtection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[hasPayloadLinks](../api/androidmanagedappprotection-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[assign](../api/androidmanagedappprotection-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/androidmanagedappprotection-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/androidmanagedappprotection-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/androidmanagedappprotection-delete-assignments.md)|None|Delete an [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|
|[Update assignments](../api/androidmanagedappprotection-update-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Update the properties of an assignments object.|
|[Get targetedManagedAppPolicyAssignment](../api/targetedmanagedapppolicyassignment-get.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Read the properties and relationships of a [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|
|[List apps](../api/androidmanagedappprotection-list-apps.md)|[managedMobileApp](../resources/managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Create apps](../api/androidmanagedappprotection-post-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Create a new apps object.|
|[Delete apps](../api/androidmanagedappprotection-delete-apps.md)|None|Delete an [managedMobileApp](../resources/managedmobileapp.md) object.|
|[Update apps](../api/androidmanagedappprotection-update-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Update the properties of an apps object.|
|[Get managedMobileApp](../api/managedmobileapp-get.md)|[managedMobileApp](../resources/managedmobileapp.md)|Read the properties and relationships of a [managedMobileApp](../resources/managedmobileapp.md) object.|
|[List deploymentSummary](../api/androidmanagedappprotection-list-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) collection|Get the managedAppPolicyDeploymentSummaries from the deploymentSummary navigation property.|
|[Create deploymentSummary](../api/androidmanagedappprotection-post-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Create a new deploymentSummary object.|
|[Delete deploymentSummary](../api/androidmanagedappprotection-delete-deploymentsummary.md)|None|Delete a [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|
|[Update deploymentSummary](../api/androidmanagedappprotection-update-deploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Update the properties of a deploymentSummary object.|
|[Get managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Read the properties and relationships of a [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAndroidDeviceManufacturers|String|**TODO: Add Description**|
|allowedAndroidDeviceModels|String collection|**TODO: Add Description**|
|allowedDataIngestionLocations|managedAppDataIngestionLocation collection|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedDataStorageLocations|managedAppDataStorageLocation collection|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedInboundDataTransferSources|managedAppDataTransferLevel|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|allowedOutboundClipboardSharingExceptionLength|Int32|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|managedAppClipboardSharingLevel|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|allowedOutboundDataTransferDestinations|managedAppDataTransferLevel|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|appActionIfAndroidDeviceManufacturerNotAllowed|managedAppRemediationAction|**TODO: Add Description**. Possible values are: `block`, `wipe`, `warn`.|
|appActionIfAndroidDeviceModelNotAllowed|managedAppRemediationAction|**TODO: Add Description**. Possible values are: `block`, `wipe`, `warn`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|managedAppRemediationAction|**TODO: Add Description**. Possible values are: `block`, `wipe`, `warn`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|managedAppRemediationAction|**TODO: Add Description**. Possible values are: `block`, `wipe`, `warn`.|
|appActionIfDeviceComplianceRequired|managedAppRemediationAction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|managedAppRemediationAction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appActionIfUnableToAuthenticateUser|managedAppRemediationAction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|approvedKeyboards|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|blockDataIngestionIntoOrganizationDocuments|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|contactSyncBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customBrowserDisplayName|String|**TODO: Add Description**|
|customBrowserPackageId|String|**TODO: Add Description**|
|dataBackupBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|deployedAppCount|Int32|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|deviceComplianceRequired|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|**TODO: Add Description**|
|disableAppPinIfDevicePinIsSet|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|encryptAppData|Boolean|**TODO: Add Description**|
|exemptedAppPackages|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|fingerprintBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isAssigned|Boolean|**TODO: Add Description** Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md)|
|keyboardsRestricted|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|managedBrowser|managedBrowserType|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `microsoftEdge`.|
|managedBrowserToOpenLinksRequired|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|maximumAllowedDeviceThreatLevel|managedAppDeviceThreatLevel|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|maximumPinRetries|Int32|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumPinLength|Int32|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredAppVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredCompanyPortalVersion|String|**TODO: Add Description**|
|minimumRequiredOsVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredPatchVersion|String|**TODO: Add Description**|
|minimumWarningAppVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningCompanyPortalVersion|String|**TODO: Add Description**|
|minimumWarningOsVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningPatchVersion|String|**TODO: Add Description**|
|minimumWipeAppVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipeCompanyPortalVersion|String|**TODO: Add Description**|
|minimumWipeOsVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipePatchVersion|String|**TODO: Add Description**|
|mobileThreatDefenseRemediationAction|managedAppRemediationAction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|notificationRestriction|managedAppNotificationRestriction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allow`, `blockOrganizationalData`, `block`.|
|organizationalCredentialsRequired|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodBeforePinReset|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOfflineBeforeAccessCheck|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinCharacterSet|managedAppPinCharacterSet|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `numeric`, `alphanumericAndSymbol`.|
|pinRequired|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinRequiredInsteadOfBiometricTimeout|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|previousPinBlockCount|Int32|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|printBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|requiredAndroidSafetyNetAppsVerificationType|androidManagedAppSafetyNetAppsVerificationType|**TODO: Add Description**. Possible values are: `none`, `enabled`.|
|requiredAndroidSafetyNetDeviceAttestationType|androidManagedAppSafetyNetDeviceAttestationType|**TODO: Add Description**. Possible values are: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|roleScopeTagIds|String collection|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|saveAsBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|screenCaptureBlocked|Boolean|**TODO: Add Description**|
|simplePinBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|targetedAppManagementLevels|appManagementLevel|**TODO: Add Description** Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md). Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/managedmobileapp.md) collection|**TODO: Add Description**|
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|**TODO: Add Description** Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md)|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppProtection",
  "baseType": "microsoft.graph.targetedManagedAppProtection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": "Boolean",
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": "Boolean",
  "deviceComplianceRequired": "Boolean",
  "managedBrowserToOpenLinksRequired": "Boolean",
  "saveAsBlocked": "Boolean",
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": "Boolean",
  "maximumPinRetries": "Integer",
  "simplePinBlocked": "Boolean",
  "minimumPinLength": "Integer",
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": "Boolean",
  "printBlocked": "Boolean",
  "fingerprintBlocked": "Boolean",
  "disableAppPinIfDevicePinIsSet": "Boolean",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": "Integer",
  "notificationRestriction": "String",
  "previousPinBlockCount": "Integer",
  "managedBrowser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "blockDataIngestionIntoOrganizationDocuments": "Boolean",
  "allowedDataIngestionLocations": [
    "String"
  ],
  "appActionIfUnableToAuthenticateUser": "String",
  "isAssigned": "Boolean",
  "targetedAppManagementLevels": "String",
  "screenCaptureBlocked": "Boolean",
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": "Boolean",
  "encryptAppData": "Boolean",
  "deployedAppCount": "Integer",
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "minimumWipePatchVersion": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String",
  "minimumRequiredCompanyPortalVersion": "String",
  "minimumWarningCompanyPortalVersion": "String",
  "minimumWipeCompanyPortalVersion": "String",
  "keyboardsRestricted": "Boolean",
  "approvedKeyboards": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "allowedAndroidDeviceModels": [
    "String"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String"
}
```

