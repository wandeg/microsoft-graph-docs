---
title: "groupPolicyPresentationText resource type"
description: "Represents an ADMX text element."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyPresentationText resource type

Represents an ADMX text element.


Inherits from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationTexts](../api/grouppolicypresentationtext-list.md)|[groupPolicyPresentationText](../resources/groupPolicyPresentationText.md) collection|List properties and relationships of the [groupPolicyPresentationText](../resources/grouppolicypresentationtext.md) objects.|
|[Get groupPolicyPresentationText](../api/grouppolicypresentationtext-get.md)|[groupPolicyPresentationText](../resources/groupPolicyPresentationText.md)|Read properties and relationships of the [groupPolicyPresentationText](../resources/grouppolicypresentationtext.md) object.|
|[Create groupPolicyPresentationText](../api/grouppolicypresentationtext-create.md)|[groupPolicyPresentationText](../resources/groupPolicyPresentationText.md)|Create a new [groupPolicyPresentationText](../resources/grouppolicypresentationtext.md) object.|
|[Delete groupPolicyPresentationText](../api/grouppolicypresentationtext-delete.md)|None|Deletes a [groupPolicyPresentationText](../resources/grouppolicypresentationtext.md).|
|[Update groupPolicyPresentationText](../api/grouppolicypresentationtext-update.md)|[groupPolicyPresentationText](../resources/groupPolicyPresentationText.md)|Update the properties of a [groupPolicyPresentationText](../resources/grouppolicypresentationtext.md) object.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|The group policy definition associated with the presentation. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationText",
  "baseType": "microsoft.graph.groupPolicyPresentation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

