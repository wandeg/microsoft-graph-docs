---
title: "groupPolicyCategory resource type"
description: "The category entity stores the category of a group policy definition"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyCategory resource type


Namespace: microsoft.graph

The category entity stores the category of a group policy definition


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyCategory](../api/grouppolicycategory-get.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Read the properties and relationships of a [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[Update groupPolicyCategory](../api/grouppolicycategory-update.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Update the properties of a [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[List parent](../api/grouppolicycategory-list-parent.md)|[groupPolicyCategory](../resources/grouppolicycategory.md) collection|Get the groupPolicyCategories from the parent navigation property.|
|[Add parent](../api/grouppolicycategory-post-parent.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Add parent by posting to the parent collection.|
|[Remove parent](../api/grouppolicycategory-delete-parent.md)|None|Remove a [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[List children](../api/grouppolicycategory-list-children.md)|[groupPolicyCategory](../resources/grouppolicycategory.md) collection|Get the groupPolicyCategories from the children navigation property.|
|[Add children](../api/grouppolicycategory-post-children.md)|[groupPolicyCategory](../resources/grouppolicycategory.md)|Add children by posting to the children collection.|
|[Remove children](../api/grouppolicycategory-delete-children.md)|None|Remove a [groupPolicyCategory](../resources/grouppolicycategory.md) object.|
|[List definitions](../api/grouppolicycategory-list-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the definitions navigation property.|
|[Add definitions](../api/grouppolicycategory-post-definitions.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Add definitions by posting to the definitions collection.|
|[Remove definitions](../api/grouppolicycategory-delete-definitions.md)|None|Remove a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[List definitionFile](../api/grouppolicycategory-list-definitionfile.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) collection|Get the groupPolicyDefinitionFiles from the definitionFile navigation property.|
|[Add definitionFile](../api/grouppolicycategory-post-definitionfile.md)|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|Add definitionFile by posting to the definitionFile collection.|
|[Remove definitionFile](../api/grouppolicycategory-delete-definitionfile.md)|None|Remove a [groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The string id of the category's display name|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isRoot|Boolean|Defines if the category is a root category|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|children|[groupPolicyCategory](../resources/grouppolicycategory.md) collection|The children categories|
|definitionFile|[groupPolicyDefinitionFile](../resources/grouppolicydefinitionfile.md)|The id of the definition file the category came from|
|definitions|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|The immediate GroupPolicyDefinition children of the category|
|parent|[groupPolicyCategory](../resources/grouppolicycategory.md)|The parent category|

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

