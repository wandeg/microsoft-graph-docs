---
title: "bitLockerRecoveryOptions resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bitLockerRecoveryOptions resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolean|Indicates whether to block certificate-based data recovery agent.|
|enableBitLockerAfterRecoveryInformationToStore|Boolean|Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.|
|enableRecoveryInformationSaveToStore|Boolean|Indicates whether or not to allow BitLocker recovery information to store in AD DS.|
|hideRecoveryOptions|Boolean|Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.|
|recoveryInformationToStore|Enumeration|Configure what pieces of BitLocker recovery information are stored to AD DS. Possible values are: `passwordAndKey`, `passwordOnly`.|
|recoveryKeyUsage|Enumeration|Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk. Possible values are: `blocked`, `required`, `allowed`.|
|recoveryPasswordUsage|Enumeration|Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk. Possible values are: `blocked`, `required`, `allowed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```

