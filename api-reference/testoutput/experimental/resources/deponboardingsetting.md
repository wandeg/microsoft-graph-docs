---
title: "depOnboardingSetting resource type"
description: "The depOnboardingSetting represents an instance of the Apple DEP service being onboarded to Intune. The onboarded service instance manages an Apple Token used to synchronize data between Apple and Intune."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# depOnboardingSetting resource type

The depOnboardingSetting represents an instance of the Apple DEP service being onboarded to Intune. The onboarded service instance manages an Apple Token used to synchronize data between Apple and Intune.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get depOnboardingSetting](../api/deponboardingsetting-get.md)|[depOnboardingSetting](../resources/depOnboardingSetting.md)|Read properties and relationships of the [depOnboardingSetting](../resources/deponboardingsetting.md) object.|
|[Delete depOnboardingSetting](../api/deponboardingsetting-delete.md)|None|Deletes a [depOnboardingSetting](../resources/deponboardingsetting.md).|
|[Update depOnboardingSetting](../api/deponboardingsetting-update.md)|[depOnboardingSetting](../resources/depOnboardingSetting.md)|Update the properties of a [depOnboardingSetting](../resources/deponboardingsetting.md) object.|
|[getEncryptionPublicKey](../api/deponboardingsetting-getencryptionpublickey.md)|String||
|[uploadDepToken](../api/deponboardingsetting-uploaddeptoken.md)|None||
|[syncWithAppleDeviceEnrollmentProgram](../api/deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|None||
|[shareForSchoolDataSyncService](../api/deponboardingsetting-shareforschooldatasyncservice.md)|None||
|[unshareForSchoolDataSyncService](../api/deponboardingsetting-unshareforschooldatasyncservice.md)|None||
|[getExpiringVppTokenCount](../api/deponboardingsetting-getexpiringvpptokencount.md)|Int32||
|[Get depIOSEnrollmentProfile](../api/depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/depIOSEnrollmentProfile.md)|Read properties and relationships of the [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.|
|[Get depMacOSEnrollmentProfile](../api/depmacosenrollmentprofile-get.md)|[depMacOSEnrollmentProfile](../resources/depMacOSEnrollmentProfile.md)|Read properties and relationships of the [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) object.|
|[List enrollmentProfiles](../api/deponboardingsetting-list-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentProfile.md) collection|Get the enrollmentProfiles from the enrollmentProfiles navigation property.|
|[Add enrollmentProfiles](../api/deponboardingsetting-post-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentProfile.md)|Add enrollmentProfiles by posting to the enrollmentProfiles collection.|
|[List importedAppleDeviceIdentities](../api/deponboardingsetting-list-importedappledeviceidentities.md)|[importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md) collection|Get the importedAppleDeviceIdentities from the importedAppleDeviceIdentities navigation property.|
|[Add importedAppleDeviceIdentities](../api/deponboardingsetting-post-importedappledeviceidentities.md)|[importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|Add importedAppleDeviceIdentities by posting to the importedAppleDeviceIdentities collection.|
|[List depOnboardingSettings](../api/intune-devices-devicemanagement-list-deponboardingsettings.md)|[depOnboardingSetting](../resources/depOnboardingSetting.md) collection|Get the depOnboardingSettings from the depOnboardingSettings navigation property.|
|[Add depOnboardingSettings](../api/intune-devices-devicemanagement-post-deponboardingsettings.md)|[depOnboardingSetting](../resources/depOnboardingSetting.md)|Add depOnboardingSettings by posting to the depOnboardingSettings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleIdentifier|String|The Apple ID used to obtain the current token.|
|dataSharingConsentGranted|Boolean|Consent granted for data sharing with Apple Dep Service|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|When the service was onboarded.|
|lastSuccessfulSyncDateTime|DateTimeOffset|When the service last syned with Intune|
|lastSyncErrorCode|Int32|Error code reported by Apple during last dep sync.|
|lastSyncTriggeredDateTime|DateTimeOffset|When Intune last requested a sync.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|shareTokenWithSchoolDataSyncService|Boolean|Whether or not the Dep token sharing is enabled with the School Data Sync service.|
|syncedDeviceCount|Int32|Gets synced device count|
|tokenExpirationDateTime|DateTimeOffset|When the token will expire.|
|tokenName|String|Friendly Name for Dep Token|
|tokenType|Enumeration|Gets or sets the Dep Token Type. Possible values are: `none`, `dep`, `appleSchoolManager`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/depIOSEnrollmentProfile.md)|Default iOS Enrollment Profile|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/depMacOSEnrollmentProfile.md)|Default MacOs Enrollment Profile|
|enrollmentProfiles|[enrollmentProfile](../resources/enrollmentProfile.md) collection|The enrollment profiles.|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md) collection|The imported Apple device identities.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depOnboardingSetting",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1024,
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": 1024,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```

