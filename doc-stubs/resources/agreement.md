---
title: "agreement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# agreement resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List agreements](../api/agreement-list.md)|[agreement](../resources/agreement.md) collection|Get a list of the [agreement](../resources/agreement.md) objects and their properties.|
|[Get agreement](../api/agreement-get.md)|[agreement](../resources/agreement.md)|Read the properties and relationships of an [agreement](../resources/agreement.md) object.|
|[Create agreement](../api/agreement-post-agreements.md)|[agreement](../resources/agreement.md)|Create a new [agreement](../resources/agreement.md) object.|
|[Delete agreement](../api/agreement-delete.md)|None|Deletes an [agreement](../resources/agreement.md) object.|
|[Update agreement](../api/agreement-update.md)|[agreement](../resources/agreement.md)|Update the properties of an [agreement](../resources/agreement.md) object.|
|[List files](../api/agreement-list-files.md)|[agreementFile](../resources/agreementfile.md) collection|Get the agreementFiles from the files navigation property.|
|[Create files](../api/agreement-post-files.md)|[agreementFile](../resources/agreementfile.md)|Create a new files object.|
|[Delete files](../api/agreement-delete-files.md)|None|Delete a [agreementFile](../resources/agreementfile.md) object.|
|[Update files](../api/agreement-update-files.md)|[agreementFile](../resources/agreementfile.md)|Update the properties of a files object.|
|[Get agreementFile](../api/agreementfile-get.md)|[agreementFile](../resources/agreementfile.md)|Read the properties and relationships of an [agreementFile](../resources/agreementfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isViewingBeforeAcceptanceRequired|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|files|[agreementFile](../resources/agreementfile.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "isViewingBeforeAcceptanceRequired": "Boolean"
}
```

