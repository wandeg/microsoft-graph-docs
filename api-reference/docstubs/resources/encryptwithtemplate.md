---
title: "encryptWithTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# encryptWithTemplate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [encryptContent](../resources/encryptcontent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableForEncryption|Boolean|**TODO: Add Description**|
|encryptWith|encryptWith|**TODO: Add Description** Inherited from [encryptContent](../resources/encryptcontent.md). Possible values are: `template`, `userDefinedRights`.|
|name|String|**TODO: Add Description** Inherited from [labelActionBase](../resources/labelactionbase.md)|
|templateId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptWithTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptWithTemplate",
  "name": "String",
  "encryptWith": "String",
  "templateId": "String",
  "availableForEncryption": true
}
```

