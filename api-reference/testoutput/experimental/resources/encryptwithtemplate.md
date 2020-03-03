---
title: "encryptWithTemplate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# encryptWithTemplate resource type




Inherits from [encryptContent](../resources/encryptContent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableForEncryption|Boolean||
|encryptWith|Enumeration| Inherited from [encryptContent](../resources/encryptContent.md). Possible values are: `template`, `userDefinedRights`.|
|name|String| Inherited from [labelActionBase](../resources/labelActionBase.md)|
|templateId|String||

## Relationships
None

## JSON Representation
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

