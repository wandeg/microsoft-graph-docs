---
title: "appLogCollectionDownloadDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appLogCollectionDownloadDetails resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appLogDecryptionAlgorithm|Enumeration| Possible values are: `aes256`.|
|decryptionKey|String||
|downloadUrl|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```

