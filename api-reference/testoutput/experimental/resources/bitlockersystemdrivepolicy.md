---
title: "bitLockerSystemDrivePolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bitLockerSystemDrivePolicy resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|encryptionMethod|Enumeration|Select the encryption method for operating system drives. Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|minimumPinLength|Int32|Indicates the minimum length of startup pin. Valid values 4 to 20|
|prebootRecoveryEnableMessageAndUrl|Boolean|Enable pre-boot recovery message and Url. If requireStartupAuthentication is false, this value does not affect.|
|prebootRecoveryMessage|String|Defines a custom recovery message.|
|prebootRecoveryUrl|String|Defines a custom recovery URL.|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/bitlockerrecoveryoptions.md)|Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information. This policy setting is applied when you turn on BitLocker.|
|startupAuthenticationBlockWithoutTpmChip|Boolean|Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).|
|startupAuthenticationRequired|Boolean|Require additional authentication at startup.|
|startupAuthenticationTpmKeyUsage|Enumeration|Indicates if TPM startup key is allowed/required/disallowed. Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|Enumeration|Indicates if TPM startup pin key and key are allowed/required/disallowed. Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinUsage|Enumeration|Indicates if TPM startup pin is allowed/required/disallowed. Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmUsage|Enumeration|Indicates if TPM startup is allowed/required/disallowed. Possible values are: `blocked`, `required`, `allowed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```

