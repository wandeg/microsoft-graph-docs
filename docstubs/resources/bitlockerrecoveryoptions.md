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
|blockDataRecoveryAgent|Boolean||
|enableBitLockerAfterRecoveryInformationToStore|Boolean||
|enableRecoveryInformationSaveToStore|Boolean||
|hideRecoveryOptions|Boolean||
|recoveryInformationToStore|Enumeration| Possible values are: `passwordAndKey`, `passwordOnly`.|
|recoveryKeyUsage|Enumeration| Possible values are: `blocked`, `required`, `allowed`.|
|recoveryPasswordUsage|Enumeration| Possible values are: `blocked`, `required`, `allowed`.|

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

