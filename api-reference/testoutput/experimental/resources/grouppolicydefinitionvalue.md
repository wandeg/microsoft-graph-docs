---
title: "groupPolicyDefinitionValue resource type"
description: "The definition value entity stores the value for a single group policy definition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyDefinitionValue resource type


Namespace: microsoft.graph

The definition value entity stores the value for a single group policy definition.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Read properties and relationships of the [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Update groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-update.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Update the properties of a [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[List presentationValues](../api/grouppolicydefinitionvalue-list-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) collection|Get the groupPolicyPresentationValues from the presentationValues navigation property.|
|[Add presentationValues](../api/grouppolicydefinitionvalue-post-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Add presentationValues by posting to the presentationValues collection.|
|[Get groupPolicyDefinition](../api/grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Read properties and relationships of the [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[List definitionValues](../api/grouppolicyconfiguration-list-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection|Get the groupPolicyDefinitionValues from the definitionValues navigation property.|
|[Add definitionValues](../api/grouppolicyconfiguration-post-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Add definitionValues by posting to the definitionValues collection.|

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
|definition|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|The associated group policy definition with the value.|
|presentationValues|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) collection|The associated group policy presentation values with the definition value.|

## JSON representation
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

