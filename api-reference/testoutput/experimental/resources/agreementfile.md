---
title: "agreementFile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# agreementFile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get agreementFile](../api/agreementfile-get.md)|[agreementFile](../resources/agreementFile.md)|Read properties and relationships of the [agreementFile](../resources/agreementfile.md) object.|
|[Delete agreementFile](../api/agreementfile-delete.md)|None|Deletes a [agreementFile](../resources/agreementfile.md).|
|[Update agreementFile](../api/agreementfile-update.md)|[agreementFile](../resources/agreementFile.md)|Update the properties of a [agreementFile](../resources/agreementfile.md) object.|
|[List files](../api/agreement-list-files.md)|[agreementFile](../resources/agreementFile.md) collection|Get the agreementFiles from the files navigation property.|
|[Add files](../api/agreement-post-files.md)|[agreementFile](../resources/agreementFile.md)|Add files by posting to the files collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fileData|[agreementFileData](../resources/agreementFileData.md)||
|fileName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|language|String||

## Relationships
None

## JSON Representation
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

