---
title: "bitLockerRemovableDrivePolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bitLockerRemovableDrivePolicy resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|blockCrossOrganizationWriteAccess|Boolean||
|encryptionMethod|Enumeration| Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|requireEncryptionForWriteAccess|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```

