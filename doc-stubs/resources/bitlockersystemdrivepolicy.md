---
title: "bitLockerSystemDrivePolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bitLockerSystemDrivePolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|encryptionMethod|bitLockerEncryptionMethod|**TODO: Add Description**. Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|minimumPinLength|Int32|**TODO: Add Description**|
|prebootRecoveryEnableMessageAndUrl|Boolean|**TODO: Add Description**|
|prebootRecoveryMessage|String|**TODO: Add Description**|
|prebootRecoveryUrl|String|**TODO: Add Description**|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/bitlockerrecoveryoptions.md)|**TODO: Add Description**|
|startupAuthenticationBlockWithoutTpmChip|Boolean|**TODO: Add Description**|
|startupAuthenticationRequired|Boolean|**TODO: Add Description**|
|startupAuthenticationTpmKeyUsage|configurationUsage|**TODO: Add Description**. Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|configurationUsage|**TODO: Add Description**. Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinUsage|configurationUsage|**TODO: Add Description**. Possible values are: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmUsage|configurationUsage|**TODO: Add Description**. Possible values are: `blocked`, `required`, `allowed`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": "Boolean",
  "startupAuthenticationBlockWithoutTpmChip": "Boolean",
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": "Integer",
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
  },
  "prebootRecoveryEnableMessageAndUrl": "Boolean",
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```

