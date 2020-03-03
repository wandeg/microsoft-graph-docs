---
title: "groupPolicyPresentationValueText resource type"
description: "The entity represents a string value for a drop-down list, combo box, or text box presentation on a policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyPresentationValueText resource type

The entity represents a string value for a drop-down list, combo box, or text box presentation on a policy definition.


Inherits from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationValueTexts](../api/grouppolicypresentationvaluetext-list.md)|[groupPolicyPresentationValueText](../resources/groupPolicyPresentationValueText.md) collection|List properties and relationships of the [groupPolicyPresentationValueText](../resources/grouppolicypresentationvaluetext.md) objects.|
|[Get groupPolicyPresentationValueText](../api/grouppolicypresentationvaluetext-get.md)|[groupPolicyPresentationValueText](../resources/groupPolicyPresentationValueText.md)|Read properties and relationships of the [groupPolicyPresentationValueText](../resources/grouppolicypresentationvaluetext.md) object.|
|[Create groupPolicyPresentationValueText](../api/grouppolicypresentationvaluetext-create.md)|[groupPolicyPresentationValueText](../resources/groupPolicyPresentationValueText.md)|Create a new [groupPolicyPresentationValueText](../resources/grouppolicypresentationvaluetext.md) object.|
|[Delete groupPolicyPresentationValueText](../api/grouppolicypresentationvaluetext-delete.md)|None|Deletes a [groupPolicyPresentationValueText](../resources/grouppolicypresentationvaluetext.md).|
|[Update groupPolicyPresentationValueText](../api/grouppolicypresentationvaluetext-update.md)|[groupPolicyPresentationValueText](../resources/groupPolicyPresentationValueText.md)|Update the properties of a [groupPolicyPresentationValueText](../resources/grouppolicypresentationvaluetext.md) object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/groupPolicyPresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created. Inherited from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified. Inherited from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|
|value|String|A string value for the associated presentation.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md)|The group policy definition value associated with the presentation value. Inherited from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|
|presentation|[groupPolicyPresentation](../resources/groupPolicyPresentation.md)|The group policy presentation associated with the presentation value. Inherited from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueText",
  "baseType": "microsoft.graph.groupPolicyPresentationValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "value": "String"
}
```

