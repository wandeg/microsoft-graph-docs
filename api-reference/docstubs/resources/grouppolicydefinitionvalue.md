---
title: "groupPolicyDefinitionValue resource type"
description: "The definition value entity stores the value for a single group policy definition."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyDefinitionValue resource type


Namespace: microsoft.graph

The definition value entity stores the value for a single group policy definition.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Read the properties and relationships of a [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Update groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-update.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Update the properties of a [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[List presentationValues](../api/grouppolicydefinitionvalue-list-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) collection|Get the groupPolicyPresentationValues from the presentationValues navigation property.|
|[Create presentationValues](../api/grouppolicydefinitionvalue-post-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Create a new presentationValues object.|
|[Delete presentationValues](../api/grouppolicydefinitionvalue-delete-presentationvalues.md)|None|Delete a [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[Update presentationValues](../api/grouppolicydefinitionvalue-update-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Update the properties of a presentationValues object.|
|[Get groupPolicyPresentationValue](../api/grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Read the properties and relationships of a [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[List definition](../api/grouppolicydefinitionvalue-list-definition.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the definition navigation property.|
|[Add definition](../api/grouppolicydefinitionvalue-post-definition.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Add definition by posting to the definition collection.|
|[Remove definition](../api/grouppolicydefinitionvalue-delete-definition.md)|None|Remove a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationType|groupPolicyConfigurationType|Specifies how the value should be configured. This can be either as a Policy or as a Preference. Possible values are: `policy`, `preference`.|
|createdDateTime|DateTimeOffset|The date and time the object was created.|
|enabled|Boolean|Enables or disables the associated group policy definition.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

