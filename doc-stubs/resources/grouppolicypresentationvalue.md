---
title: "groupPolicyPresentationValue resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyPresentationValue resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List definitionValue](../api/grouppolicypresentationvalue-list-definitionvalue.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection|Get the groupPolicyDefinitionValues from the definitionValue navigation property.|
|[Add definitionValue](../api/grouppolicypresentationvalue-post-definitionvalue.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Add definitionValue by posting to the definitionValue collection.|
|[Remove definitionValue](../api/grouppolicypresentationvalue-delete-definitionvalue.md)|None|Remove a [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[List presentation](../api/grouppolicypresentationvalue-list-presentation.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection|Get the groupPolicyPresentations from the presentation navigation property.|
|[Add presentation](../api/grouppolicypresentationvalue-post-presentation.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Add presentation by posting to the presentation collection.|
|[Remove presentation](../api/grouppolicypresentationvalue-delete-presentation.md)|None|Remove a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[List presentationValues](../api/grouppolicydefinitionvalue-list-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) collection|Get the groupPolicyPresentationValues from the presentationValues navigation property.|
|[Create presentationValues](../api/grouppolicydefinitionvalue-post-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Create a new presentationValues object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|**TODO: Add Description**|
|presentation|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```

