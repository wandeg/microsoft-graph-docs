---
title: "groupPolicyPresentation resource type"
description: "The base entity for the display presentation of any of the additional options in a group policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentation resource type


Namespace: microsoft.graph

The base entity for the display presentation of any of the additional options in a group policy definition.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Update groupPolicyPresentation](../api/grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Update the properties of a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[List presentations](../api/grouppolicydefinition-list-presentations.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection|Get the groupPolicyPresentations from the presentations navigation property.|
|[Add presentations](../api/grouppolicydefinition-post-presentations.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Add presentations by posting to the presentations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
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

