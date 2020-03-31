---
title: "encryptWithTemplate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# encryptWithTemplate resource type


Namespace: microsoft.graph




Inherits from [encryptContent](../resources/encryptcontent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableForEncryption|Boolean||
|encryptWith|Enumeration| Inherited from [encryptContent](../resources/encryptcontent.md). Possible values are: `template`, `userDefinedRights`.|
|name|String| Inherited from [labelActionBase](../resources/labelactionbase.md)|
|templateId|String||

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

