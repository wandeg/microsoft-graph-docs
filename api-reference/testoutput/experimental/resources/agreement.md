---
title: "agreement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# agreement resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List agreements](../api/agreement-list.md)|[agreement](../resources/agreement.md) collection|List properties and relationships of the [agreement](../resources/agreement.md) objects.|
|[Get agreement](../api/agreement-get.md)|[agreement](../resources/agreement.md)|Read properties and relationships of the [agreement](../resources/agreement.md) object.|
|[Create agreement](../api/agreement-post-agreements.md)|[agreement](../resources/agreement.md)|Create a new [agreement](../resources/agreement.md) object.|
|[Delete agreement](../api/agreement-delete.md)|None|Deletes a [agreement](../resources/agreement.md).|
|[Update agreement](../api/agreement-update.md)|[agreement](../resources/agreement.md)|Update the properties of a [agreement](../resources/agreement.md) object.|
|[List files](../api/agreement-list-files.md)|[agreementFile](../resources/agreementfile.md) collection|Get the agreementFiles from the files navigation property.|
|[Add files](../api/agreement-post-files.md)|[agreementFile](../resources/agreementfile.md)|Add files by posting to the files collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isViewingBeforeAcceptanceRequired|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|files|[agreementFile](../resources/agreementfile.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreement",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreement",
  "id": "String (identifier)",
  "displayName": "String",
  "isViewingBeforeAcceptanceRequired": true
}
```

