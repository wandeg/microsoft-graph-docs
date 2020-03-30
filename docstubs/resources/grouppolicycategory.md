---
title: "groupPolicyCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyCategory resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyCategory](../api/grouppolicycategory-get.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Read properties and relationships of the [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[Update groupPolicyCategory](../api/grouppolicycategory-update.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Update the properties of a [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[Get groupPolicyCategory](../api/grouppolicycategory-get.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Read properties and relationships of the [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[List children](../api/grouppolicycategory-list-children.md)|[groupPolicyCategory](../resources/grouppolicycategory.md) collection|Get the groupPolicyCategories from the children navigation property.|
|[Create children](../api/grouppolicycategory-post-children.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Create children by posting to the children collection.|
|[List definitions](../api/grouppolicycategory-list-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the definitions navigation property.|
|[Create definitions](../api/grouppolicycategory-post-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Create definitions by posting to the definitions collection.|
|[Get groupPolicyDefinitionFile](../api/grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Read properties and relationships of the [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isRoot|Boolean||
|lastModifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|children|[groupPolicyCategory](../resources/grouppolicycategory.md) collection||
|definitionFile|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)||
|definitions|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection||
|parent|[groupPolicyCategory](../resources/grouppolicycategory.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "isRoot": true,
  "lastModifiedDateTime": "String (timestamp)"
}
```

