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
|[List agreementFiles](../api/agreementfile-list.md)|[agreementFile](../resources/agreementfile.md) collection|List properties and relationships of the [agreementFile](../resources/agreementfile.md) objects.|
|[Get agreementFile](../api/agreementfile-get.md)|[agreementFile](../resources/agreementfile.md)|Read properties and relationships of the [agreementFile](../resources/agreementfile.md) object.|
|[Create agreementFile](../api/agreementfile-create.md)|[agreementFile](../resources/agreementfile.md)|Create a new [agreementFile](../resources/agreementfile.md) object.|
|[Delete agreementFile](../api/agreementfile-delete.md)|None|Deletes a [agreementFile](../resources/agreementfile.md).|
|[Update agreementFile](../api/agreementfile-update.md)|[agreementFile](../resources/agreementfile.md)|Update the properties of a [agreementFile](../resources/agreementfile.md) object.|
|[List files](../api/agreement-list-files.md)|[agreementFile](../resources/agreementfile.md) collection|Get the agreementFiles from the files navigation property.|
|[Add files](../api/agreement-post-files.md)|[agreementFile](../resources/agreementfile.md)|Add files by posting to the files collection.|

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

