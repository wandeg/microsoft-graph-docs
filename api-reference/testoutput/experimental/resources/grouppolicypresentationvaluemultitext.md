---
title: "groupPolicyPresentationValueMultiText resource type"
description: "The entity represents a string value of a multi-line text box presentation on a policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentationValueMultiText resource type


Namespace: microsoft.graph

The entity represents a string value of a multi-line text box presentation on a policy definition.


Inherits from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationValueMultiTexts](../api/grouppolicypresentationvaluemultitext-list.md)|[groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) collection|List properties and relationships of the [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) objects.|
|[Get groupPolicyPresentationValueMultiText](../api/grouppolicypresentationvaluemultitext-get.md)|[groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md)|Read properties and relationships of the [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) object.|
|[Create groupPolicyPresentationValueMultiText](../api/grouppolicypresentationvaluemultitext-create.md)|[groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md)|Create a new [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) object.|
|[Delete groupPolicyPresentationValueMultiText](../api/grouppolicypresentationvaluemultitext-delete.md)|None|Deletes a [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md).|
|[Update groupPolicyPresentationValueMultiText](../api/grouppolicypresentationvaluemultitext-update.md)|[groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md)|Update the properties of a [groupPolicyPresentationValueMultiText](../resources/grouppolicypresentationvaluemultitext.md) object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|values|String collection|A collection of non-empty strings for the associated presentation.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|The group policy definition value associated with the presentation value. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|presentation|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|The group policy presentation associated with the presentation value. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueMultiText",
  "baseType": "microsoft.graph.groupPolicyPresentationValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "values": [
    "String"
  ]
}
```

