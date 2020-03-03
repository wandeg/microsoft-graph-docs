---
title: "groupPolicyPresentationValueBoolean resource type"
description: "The entity represents a Boolean value of a checkbox presentation on a policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentationValueBoolean resource type


Namespace: microsoft.graph

The entity represents a Boolean value of a checkbox presentation on a policy definition.


Inherits from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationValueBooleans](../api/grouppolicypresentationvalueboolean-list.md)|[groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) collection|List properties and relationships of the [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) objects.|
|[Get groupPolicyPresentationValueBoolean](../api/grouppolicypresentationvalueboolean-get.md)|[groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md)|Read properties and relationships of the [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) object.|
|[Create groupPolicyPresentationValueBoolean](../api/grouppolicypresentationvalueboolean-create.md)|[groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md)|Create a new [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) object.|
|[Delete groupPolicyPresentationValueBoolean](../api/grouppolicypresentationvalueboolean-delete.md)|None|Deletes a [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md).|
|[Update groupPolicyPresentationValueBoolean](../api/grouppolicypresentationvalueboolean-update.md)|[groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md)|Update the properties of a [groupPolicyPresentationValueBoolean](../resources/grouppolicypresentationvalueboolean.md) object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified. Inherited from [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|
|value|Boolean|An boolean value for the associated presentation.|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueBoolean",
  "baseType": "microsoft.graph.groupPolicyPresentationValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "value": true
}
```

