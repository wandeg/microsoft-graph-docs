---
title: "groupPolicyDefinitionValue resource type"
description: "The definition value entity stores the value for a single group policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyDefinitionValue resource type

The definition value entity stores the value for a single group policy definition.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Delete groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-delete.md)|None|Deletes a [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md).|
|[Update groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-update.md)|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md)|Update the properties of a [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[List presentationValues](../api/grouppolicydefinitionvalue-list-presentationvalues.md)|[groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md) collection|Get the groupPolicyPresentationValues from the presentationValues navigation property.|
|[Add presentationValues](../api/grouppolicydefinitionvalue-post-presentationvalues.md)|[groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md)|Add presentationValues by posting to the presentationValues collection.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationType|Enumeration|Specifies how the value should be configured. This can be either as a Policy or as a Preference. Possible values are: `policy`, `preference`.|
|createdDateTime|DateTimeOffset|The date and time the object was created.|
|enabled|Boolean|Enables or disables the associated group policy definition.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/groupPolicyDefinition.md)|The associated group policy definition with the value.|
|presentationValues|[groupPolicyPresentationValue](../resources/groupPolicyPresentationValue.md) collection|The associated group policy presentation values with the definition value.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionValue",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "enabled": true,
  "configurationType": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

