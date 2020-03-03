---
title: "groupPolicyPresentationValueDecimal resource type"
description: "The entity represents an unsigned integer value of a decimal text box presentation on a policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyPresentationValueDecimal resource type

The entity represents an unsigned integer value of a decimal text box presentation on a policy definition.


Inherits from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationValueDecimals](../api/grouppolicypresentationvaluedecimal-list.md)|[groupPolicyPresentationValueDecimal](../resources/groupPolicyPresentationValueDecimal.md) collection|List properties and relationships of the [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) objects.|
|[Get groupPolicyPresentationValueDecimal](../api/grouppolicypresentationvaluedecimal-get.md)|[groupPolicyPresentationValueDecimal](../resources/groupPolicyPresentationValueDecimal.md)|Read properties and relationships of the [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) object.|
|[Create groupPolicyPresentationValueDecimal](../api/grouppolicypresentationvaluedecimal-create.md)|[groupPolicyPresentationValueDecimal](../resources/groupPolicyPresentationValueDecimal.md)|Create a new [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) object.|
|[Delete groupPolicyPresentationValueDecimal](../api/grouppolicypresentationvaluedecimal-delete.md)|None|Deletes a [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md).|
|[Update groupPolicyPresentationValueDecimal](../api/grouppolicypresentationvaluedecimal-update.md)|[groupPolicyPresentationValueDecimal](../resources/groupPolicyPresentationValueDecimal.md)|Update the properties of a [groupPolicyPresentationValueDecimal](../resources/grouppolicypresentationvaluedecimal.md) object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/groupPolicyPresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created. Inherited from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified. Inherited from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|
|value|Int64|An unsigned integer value for the associated presentation.|

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

