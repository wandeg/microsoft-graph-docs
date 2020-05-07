---
title: "appLogCollectionDownloadDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appLogCollectionDownloadDetails resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appLogDecryptionAlgorithm|appLogDecryptionAlgorithm|DecryptionAlgorithm for Content. Possible values are: `aes256`.|
|decryptionKey|String|DecryptionKey as string|
|downloadUrl|String|Download SAS Url for completed AppLogUploadRequest|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```

