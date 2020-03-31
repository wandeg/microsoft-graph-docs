---
title: "managedDeviceEncryptionState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDeviceEncryptionState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDeviceEncryptionState](../api/manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md)|Read properties and relationships of the [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) object.|
|[Update managedDeviceEncryptionState](../api/manageddeviceencryptionstate-update.md)|[managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md)|Update the properties of a [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|advancedBitLockerStates|Enumeration| Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.|
|deviceName|String||
|deviceType|Enumeration| Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|encryptionPolicySettingState|Enumeration| Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|encryptionReadinessState|Enumeration| Possible values are: `notReady`, `ready`.|
|encryptionState|Enumeration| Possible values are: `notEncrypted`, `encrypted`.|
|fileVaultStates|Enumeration| Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|osVersion|String||
|policyDetails|[encryptionReportPolicyDetails](../resources/encryptionreportpolicydetails.md) collection||
|tpmSpecificationVersion|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "deviceType": "String",
  "osVersion": "String",
  "tpmSpecificationVersion": "String",
  "deviceName": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "fileVaultStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
    }
  ]
}
```

