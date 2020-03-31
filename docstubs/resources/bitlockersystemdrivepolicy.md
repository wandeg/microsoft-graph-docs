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
|encryptionMethod|Enumeration| Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|minimumPinLength|Int32||
|prebootRecoveryEnableMessageAndUrl|Boolean||
|prebootRecoveryMessage|String||
|prebootRecoveryUrl|String||
|recoveryOptions|[bitLockerRecoveryOptions](../resources/bitlockerrecoveryoptions.md)||
|startupAuthenticationBlockWithoutTpmChip|Boolean||
|startupAuthenticationRequired|Boolean||
|startupAuthenticationTpmKeyUsage|Enumeration| Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|Enumeration| Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinUsage|Enumeration| Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmUsage|Enumeration| Possible values are: `blocked`, `required`, `allowed`.|

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

