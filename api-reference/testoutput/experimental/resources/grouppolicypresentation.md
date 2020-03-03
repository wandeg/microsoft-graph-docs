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
|[List groupPolicyPresentations](../api/grouppolicypresentation-list.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection|List properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) objects.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Create groupPolicyPresentation](../api/grouppolicypresentation-create.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Create a new [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Delete groupPolicyPresentation](../api/grouppolicypresentation-delete.md)|None|Deletes a [groupPolicyPresentation](../resources/grouppolicypresentation.md).|
|[Update groupPolicyPresentation](../api/grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Update the properties of a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

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

## JSON Representation
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

