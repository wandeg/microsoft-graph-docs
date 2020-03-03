---
title: "appLogCollectionDownloadDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# appLogCollectionDownloadDetails resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appLogDecryptionAlgorithm|Enumeration|DecryptionAlgorithm for Content. Possible values are: `aes256`.|
|decryptionKey|String|DecryptionKey as string|
|downloadUrl|String|Download SAS Url for completed AppLogUploadRequest|

## Relationships
None

## JSON Representation
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

