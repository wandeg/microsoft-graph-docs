---
title: "groupPolicyPresentationValueDecimal resource type"
description: "The entity represents an unsigned integer value of a decimal text box presentation on a policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentationValueDecimal resource type


Namespace: microsoft.graph

The entity represents an unsigned integer value of a decimal text box presentation on a policy definition.


Inherits from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationValueDecimals](../api/grouppolicypresentationvaluedecimal-list.md)|[groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) collection|List properties and relationships of the [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) objects.|
|[Get groupPolicyPresentationValueDecimal](../api/grouppolicypresentationvaluedecimal-get.md)|[groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md)|Read properties and relationships of the [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) object.|
|[Create groupPolicyPresentationValueDecimal](../api/grouppolicypresentationvaluedecimal-create.md)|[groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md)|Create a new [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) object.|
|[Delete groupPolicyPresentationValueDecimal](../api/grouppolicypresentationvaluedecimal-delete.md)|None|Deletes a [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md).|
|[Update groupPolicyPresentationValueDecimal](../api/grouppolicypresentationvaluedecimal-update.md)|[groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md)|Update the properties of a [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|value|Int64|An unsigned integer value for the associated presentation.|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueDecimal",
  "baseType": "microsoft.graph.groupPolicyPresentationValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "value": 1024
}
```

