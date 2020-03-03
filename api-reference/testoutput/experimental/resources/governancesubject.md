---
title: "governanceSubject resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# governanceSubject resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceSubjects](../api/governancesubject-list.md)|[governanceSubject](../resources/governancesubject.md) collection|List properties and relationships of the [governanceSubject](../resources/governancesubject.md) objects.|
|[Get governanceSubject](../api/governancesubject-get.md)|[governanceSubject](../resources/governancesubject.md)|Read properties and relationships of the [governanceSubject](../resources/governancesubject.md) object.|
|[Create governanceSubject](../api/governancesubject-post-governancesubjects.md)|[governanceSubject](../resources/governancesubject.md)|Create a new [governanceSubject](../resources/governancesubject.md) object.|
|[Delete governanceSubject](../api/governancesubject-delete.md)|None|Deletes a [governanceSubject](../resources/governancesubject.md).|
|[Update governanceSubject](../api/governancesubject-update.md)|[governanceSubject](../resources/governancesubject.md)|Update the properties of a [governanceSubject](../resources/governancesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|email|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|principalName|String||
|type|String||

## Relationships
None

## JSON Representation
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

