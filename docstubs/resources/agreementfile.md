---
title: "agreementFile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# agreementFile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get agreementFile](../api/agreementfile-get.md)|[agreementFile](../resources/agreementfile.md)|Read properties and relationships of the [agreementFile](../resources/agreementfile.md) object.|
|[Update agreementFile](../api/agreementfile-update.md)|[agreementFile](../resources/agreementfile.md)|Update the properties of a [agreementFile](../resources/agreementfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fileData|[agreementFileData](../resources/agreementfiledata.md)||
|fileName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|language|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreementFile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreementFile",
  "id": "String (identifier)",
  "language": "String",
  "fileName": "String",
  "fileData": {
    "@odata.type": "microsoft.graph.agreementFileData"
  },
  "isDefault": true
}
```

