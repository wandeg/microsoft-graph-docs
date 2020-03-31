---
title: "Add managedDeviceEncryptionStates"
description: "Add managedDeviceEncryptionStates by posting to the managedDeviceEncryptionStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add managedDeviceEncryptionStates

Namespace: microsoft.graph

Add managedDeviceEncryptionStates by posting to the managedDeviceEncryptionStates collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) object.

The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String||
|deviceType|Enumeration| Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|osVersion|String||
|tpmSpecificationVersion|String||
|deviceName|String||
|encryptionReadinessState|Enumeration| Possible values are: `notReady`, `ready`.|
|encryptionState|Enumeration| Possible values are: `notEncrypted`, `encrypted`.|
|encryptionPolicySettingState|Enumeration| Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|advancedBitLockerStates|Enumeration| Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.|
|fileVaultStates|Enumeration| Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.|
|policyDetails|[encryptionReportPolicyDetails](../resources/encryptionreportpolicydetails.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_manageddeviceencryptionstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
Content-type: application/json
Content-length: 671

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "String",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "fileVaultStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.manageddeviceencryptionstate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 720

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "80b5d971-d971-80b5-71d9-b58071d9b580",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "String",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "fileVaultStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

