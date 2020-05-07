---
title: "depOnboardingSetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# depOnboardingSetting resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[getEncryptionPublicKey](../api/deponboardingsetting-getencryptionpublickey.md)|String|**TODO: Add Description**|
|[generateEncryptionPublicKey](../api/deponboardingsetting-generateencryptionpublickey.md)|String|**TODO: Add Description**|
|[uploadDepToken](../api/deponboardingsetting-uploaddeptoken.md)|None|**TODO: Add Description**|
|[syncWithAppleDeviceEnrollmentProgram](../api/deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|None|**TODO: Add Description**|
|[shareForSchoolDataSyncService](../api/deponboardingsetting-shareforschooldatasyncservice.md)|None|**TODO: Add Description**|
|[unshareForSchoolDataSyncService](../api/deponboardingsetting-unshareforschooldatasyncservice.md)|None|**TODO: Add Description**|
|[getExpiringVppTokenCount](../api/deponboardingsetting-getexpiringvpptokencount.md)|Int32|**TODO: Add Description**|
|[List defaultIosEnrollmentProfile](../api/deponboardingsetting-list-defaultiosenrollmentprofile.md)|[depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) collection|Get the depIOSEnrollmentProfiles from the defaultIosEnrollmentProfile navigation property.|
|[Add defaultIosEnrollmentProfile](../api/deponboardingsetting-post-defaultiosenrollmentprofile.md)|[depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md)|Add defaultIosEnrollmentProfile by posting to the defaultIosEnrollmentProfile collection.|
|[Remove defaultIosEnrollmentProfile](../api/deponboardingsetting-delete-defaultiosenrollmentprofile.md)|None|Remove a [depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md) object.|
|[List defaultMacOsEnrollmentProfile](../api/deponboardingsetting-list-defaultmacosenrollmentprofile.md)|[depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) collection|Get the depMacOSEnrollmentProfiles from the defaultMacOsEnrollmentProfile navigation property.|
|[Add defaultMacOsEnrollmentProfile](../api/deponboardingsetting-post-defaultmacosenrollmentprofile.md)|[depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md)|Add defaultMacOsEnrollmentProfile by posting to the defaultMacOsEnrollmentProfile collection.|
|[Remove defaultMacOsEnrollmentProfile](../api/deponboardingsetting-delete-defaultmacosenrollmentprofile.md)|None|Remove a [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) object.|
|[List enrollmentProfiles](../api/deponboardingsetting-list-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentprofile.md) collection|Get the enrollmentProfiles from the enrollmentProfiles navigation property.|
|[Create enrollmentProfiles](../api/deponboardingsetting-post-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentprofile.md)|Create a new enrollmentProfiles object.|
|[Delete enrollmentProfiles](../api/deponboardingsetting-delete-enrollmentprofiles.md)|None|Delete an [enrollmentProfile](../resources/enrollmentprofile.md) object.|
|[Update enrollmentProfiles](../api/deponboardingsetting-update-enrollmentprofiles.md)|[enrollmentProfile](../resources/enrollmentprofile.md)|Update the properties of an enrollmentProfiles object.|
|[Get enrollmentProfile](../api/enrollmentprofile-get.md)|[enrollmentProfile](../resources/enrollmentprofile.md)|Read the properties and relationships of an [enrollmentProfile](../resources/enrollmentprofile.md) object.|
|[List importedAppleDeviceIdentities](../api/deponboardingsetting-list-importedappledeviceidentities.md)|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) collection|Get the importedAppleDeviceIdentities from the importedAppleDeviceIdentities navigation property.|
|[Create importedAppleDeviceIdentities](../api/deponboardingsetting-post-importedappledeviceidentities.md)|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|Create a new importedAppleDeviceIdentities object.|
|[Delete importedAppleDeviceIdentities](../api/deponboardingsetting-delete-importedappledeviceidentities.md)|None|Delete an [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.|
|[Update importedAppleDeviceIdentities](../api/deponboardingsetting-update-importedappledeviceidentities.md)|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|Update the properties of an importedAppleDeviceIdentities object.|
|[Get importedAppleDeviceIdentity](../api/importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|Read the properties and relationships of an [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleIdentifier|String|**TODO: Add Description**|
|dataSharingConsentGranted|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSuccessfulSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncErrorCode|Int32|**TODO: Add Description**|
|lastSyncTriggeredDateTime|DateTimeOffset|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|shareTokenWithSchoolDataSyncService|Boolean|**TODO: Add Description**|
|syncedDeviceCount|Int32|**TODO: Add Description**|
|tokenExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|tokenName|String|**TODO: Add Description**|
|tokenType|depTokenType|**TODO: Add Description**. Possible values are: `none`, `dep`, `appleSchoolManager`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/depiosenrollmentprofile.md)|**TODO: Add Description**|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md)|**TODO: Add Description**|
|enrollmentProfiles|[enrollmentProfile](../resources/enrollmentprofile.md) collection|**TODO: Add Description**|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "shareTokenWithSchoolDataSyncService": "Boolean",
  "lastSyncErrorCode": "Integer",
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": "Integer",
  "dataSharingConsentGranted": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

