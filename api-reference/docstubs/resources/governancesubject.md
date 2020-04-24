---
title: "governanceSubject resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# governanceSubject resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceSubjects](../api/governancesubject-list.md)|[governanceSubject](../resources/governancesubject.md) collection|Get a list of the [governanceSubject](../resources/governancesubject.md) objects and their properties.|
|[Get governanceSubject](../api/governancesubject-get.md)|[governanceSubject](../resources/governancesubject.md)|Read the properties and relationships of a [governanceSubject](../resources/governancesubject.md) object.|
|[Create governanceSubject](../api/governancesubject-post-governancesubjects.md)|[governanceSubject](../resources/governancesubject.md)|Create a new [governanceSubject](../resources/governancesubject.md) object.|
|[Delete governanceSubject](../api/governancesubject-delete.md)|None|Deletes a [governanceSubject](../resources/governancesubject.md) object.|
|[Update governanceSubject](../api/governancesubject-update.md)|[governanceSubject](../resources/governancesubject.md)|Update the properties of a [governanceSubject](../resources/governancesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|principalName|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.governanceSubject",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceSubject",
  "id": "String (identifier)",
  "type": "String",
  "displayName": "String",
  "principalName": "String",
  "email": "String"
}
```

