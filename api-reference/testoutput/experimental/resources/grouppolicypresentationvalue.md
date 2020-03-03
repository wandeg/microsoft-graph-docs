---
title: "groupPolicyPresentationValue resource type"
description: "The base presentation value entity that stores the value for a single group policy presentation."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentationValue resource type


Namespace: microsoft.graph

The base presentation value entity that stores the value for a single group policy presentation.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationValues](../api/grouppolicypresentationvalue-list.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) collection|List properties and relationships of the [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) objects.|
|[Get groupPolicyPresentationValue](../api/grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Read properties and relationships of the [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[Create groupPolicyPresentationValue](../api/grouppolicypresentationvalue-create.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Create a new [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[Delete groupPolicyPresentationValue](../api/grouppolicypresentationvalue-delete.md)|None|Deletes a [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md).|
|[Update groupPolicyPresentationValue](../api/grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Update the properties of a [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|The group policy definition value associated with the presentation value.|
|presentation|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|The group policy presentation associated with the presentation value.|

## JSON Representation
Here is a JSON representation of the resource.
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

