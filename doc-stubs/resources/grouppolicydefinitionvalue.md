---
title: "groupPolicyDefinitionValue resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyDefinitionValue resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List presentationValues](../api/grouppolicydefinitionvalue-list-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) collection|Get the groupPolicyPresentationValues from the presentationValues navigation property.|
|[Create presentationValues](../api/grouppolicydefinitionvalue-post-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Create a new presentationValues object.|
|[Delete presentationValues](../api/grouppolicydefinitionvalue-delete-presentationvalues.md)|None|Delete a [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[Update presentationValues](../api/grouppolicydefinitionvalue-update-presentationvalues.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Update the properties of a presentationValues object.|
|[Get groupPolicyPresentationValue](../api/grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md)|Read the properties and relationships of a [groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) object.|
|[List definition](../api/grouppolicydefinitionvalue-list-definition.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinitions from the definition navigation property.|
|[Add definition](../api/grouppolicydefinitionvalue-post-definition.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Add definition by posting to the definition collection.|
|[Remove definition](../api/grouppolicydefinitionvalue-delete-definition.md)|None|Remove a [groupPolicyDefinition](../resources/grouppolicydefinition.md) object.|
|[List definitionValues](../api/grouppolicyconfiguration-list-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection|Get the groupPolicyDefinitionValues from the definitionValues navigation property.|
|[Create definitionValues](../api/grouppolicyconfiguration-post-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Create a new definitionValues object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationType|groupPolicyConfigurationType|**TODO: Add Description**. Possible values are: `policy`, `preference`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|enabled|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|**TODO: Add Description**|
|presentationValues|[groupPolicyPresentationValue](../resources/grouppolicypresentationvalue.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "enabled": "Boolean",
  "configurationType": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

