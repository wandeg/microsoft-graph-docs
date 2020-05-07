---
title: "groupPolicyConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/grouppolicyconfiguration-assign.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) collection|**TODO: Add Description**|
|[updateDefinitionValues](../api/grouppolicyconfiguration-updatedefinitionvalues.md)|None|**TODO: Add Description**|
|[List definitionValues](../api/grouppolicyconfiguration-list-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection|Get the groupPolicyDefinitionValues from the definitionValues navigation property.|
|[Create definitionValues](../api/grouppolicyconfiguration-post-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Create a new definitionValues object.|
|[Delete definitionValues](../api/grouppolicyconfiguration-delete-definitionvalues.md)|None|Delete a [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[Update definitionValues](../api/grouppolicyconfiguration-update-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Update the properties of a definitionValues object.|
|[Get groupPolicyDefinitionValue](../api/grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Read the properties and relationships of a [groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) object.|
|[List assignments](../api/grouppolicyconfiguration-list-assignments.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) collection|Get the groupPolicyConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/grouppolicyconfiguration-post-assignments.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/grouppolicyconfiguration-delete-assignments.md)|None|Delete an [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|
|[Update assignments](../api/grouppolicyconfiguration-update-assignments.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-get.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Read the properties and relationships of a [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) collection|**TODO: Add Description**|
|definitionValues|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "lastModifiedDateTime": "String (timestamp)"
}
```

