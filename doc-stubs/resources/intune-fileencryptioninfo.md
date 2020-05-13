---
title: "fileEncryptionInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# fileEncryptionInfo resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|encryptionKey|Binary|**TODO: Add Description**|
|fileDigest|Binary|**TODO: Add Description**|
|fileDigestAlgorithm|String|**TODO: Add Description**|
|initializationVector|Binary|**TODO: Add Description**|
|mac|Binary|**TODO: Add Description**|
|macKey|Binary|**TODO: Add Description**|
|profileIdentifier|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "Binary",
  "initializationVector": "Binary",
  "mac": "Binary",
  "macKey": "Binary",
  "profileIdentifier": "String",
  "fileDigest": "Binary",
  "fileDigestAlgorithm": "String"
}
```

