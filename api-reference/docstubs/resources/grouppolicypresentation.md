---
title: "groupPolicyPresentation resource type"
description: "The base entity for the display presentation of any of the additional options in a group policy definition."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyPresentation resource type


Namespace: microsoft.graph

The base entity for the display presentation of any of the additional options in a group policy definition.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read the properties and relationships of a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Update groupPolicyPresentation](../api/grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Update the properties of a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[List definition](../api/grouppolicypresentation-list-definition.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the definition navigation property.|
|[Add definition](../api/grouppolicypresentation-post-definition.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Add definition by posting to the definition collection.|
|[Remove definition](../api/grouppolicypresentation-delete-definition.md)|None|Remove a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty.|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|The group policy definition associated with the presentation.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

