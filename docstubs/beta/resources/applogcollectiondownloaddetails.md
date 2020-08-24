---
title: "appLogCollectionDownloadDetails resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# appLogCollectionDownloadDetails resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property                  | Type   | Description                                        |
| :------------------------ | :----- | :------------------------------------------------- |
| appLogDecryptionAlgorithm | String | DecryptionAlgorithm for Content                    |
| decryptionKey             | String | DecryptionKey as string                            |
| downloadUrl               | String | Download SAS Url for completed AppLogUploadRequest |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "appLogDecryptionAlgorithm": "aes256",
  "decryptionKey": "String",
  "downloadUrl": "String"
}
```