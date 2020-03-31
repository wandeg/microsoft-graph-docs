---
title: "groupPolicyPresentationValue resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyPresentationValue resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyPresentationValue](../api/grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Read properties and relationships of the [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[Update groupPolicyPresentationValue](../api/grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Update the properties of a [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[List presentationValues](../api/grouppolicydefinitionvalue-list-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) collection|Get the groupPolicyPresentationValues from the presentationValues navigation property.|
|[Add presentationValues](../api/grouppolicydefinitionvalue-post-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Add presentationValues by posting to the presentationValues collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)||
|presentation|[groupPolicyPresentation](../resources/grouppolicypresentation.md)||

## JSON representation
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

