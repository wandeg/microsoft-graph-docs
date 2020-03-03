---
title: "groupPolicyPresentationValueList resource type"
description: "The entity represents a collection of name/value pairs of a list box presentation on a policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyPresentationValueList resource type

The entity represents a collection of name/value pairs of a list box presentation on a policy definition.


Inherits from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationValueLists](../api/grouppolicypresentationvaluelist-list.md)|[groupPolicyPresentationValueList](../resources/groupPolicyPresentationValueList.md) collection|List properties and relationships of the [groupPolicyPresentationValueList](../resources/grouppolicypresentationvaluelist.md) objects.|
|[Get groupPolicyPresentationValueList](../api/grouppolicypresentationvaluelist-get.md)|[groupPolicyPresentationValueList](../resources/groupPolicyPresentationValueList.md)|Read properties and relationships of the [groupPolicyPresentationValueList](../resources/grouppolicypresentationvaluelist.md) object.|
|[Create groupPolicyPresentationValueList](../api/grouppolicypresentationvaluelist-create.md)|[groupPolicyPresentationValueList](../resources/groupPolicyPresentationValueList.md)|Create a new [groupPolicyPresentationValueList](../resources/grouppolicypresentationvaluelist.md) object.|
|[Delete groupPolicyPresentationValueList](../api/grouppolicypresentationvaluelist-delete.md)|None|Deletes a [groupPolicyPresentationValueList](../resources/grouppolicypresentationvaluelist.md).|
|[Update groupPolicyPresentationValueList](../api/grouppolicypresentationvaluelist-update.md)|[groupPolicyPresentationValueList](../resources/groupPolicyPresentationValueList.md)|Update the properties of a [groupPolicyPresentationValueList](../resources/grouppolicypresentationvaluelist.md) object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/groupPolicyPresentation.md)|Read properties and relationships of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created. Inherited from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the object was last modified. Inherited from [groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|
|values|[keyValuePair](../resources/keyValuePair.md) collection|A list of pairs for the associated presentation.|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueList",
  "baseType": "microsoft.graph.groupPolicyPresentationValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```

