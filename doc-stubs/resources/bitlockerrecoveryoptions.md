---
title: "bitLockerRecoveryOptions resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bitLockerRecoveryOptions resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolean|**TODO: Add Description**|
|enableBitLockerAfterRecoveryInformationToStore|Boolean|**TODO: Add Description**|
|enableRecoveryInformationSaveToStore|Boolean|**TODO: Add Description**|
|hideRecoveryOptions|Boolean|**TODO: Add Description**|
|recoveryInformationToStore|bitLockerRecoveryInformationType|**TODO: Add Description**. Possible values are: `passwordAndKey`, `passwordOnly`.|
|recoveryKeyUsage|configurationUsage|**TODO: Add Description**. Possible values are: `blocked`, `required`, `allowed`.|
|recoveryPasswordUsage|configurationUsage|**TODO: Add Description**. Possible values are: `blocked`, `required`, `allowed`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": "Boolean",
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": "Boolean",
  "enableRecoveryInformationSaveToStore": "Boolean",
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": "Boolean"
}
```

