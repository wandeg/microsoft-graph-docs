---
title: "groupPolicyConfiguration resource type"
description: "The group policy configuration entity contains the configured values for one or more group policy definitions."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyConfiguration resource type


Namespace: microsoft.graph

The group policy configuration entity contains the configured values for one or more group policy definitions.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyConfigurations](../api/grouppolicyconfiguration-list.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) collection|List properties and relationships of the [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) objects.|
|[Get groupPolicyConfiguration](../api/grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md)|Read properties and relationships of the [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object.|
|[Create groupPolicyConfiguration](../api/grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md)|Create a new [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object.|
|[Delete groupPolicyConfiguration](../api/grouppolicyconfiguration-delete.md)|None|Deletes a [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md).|
|[Update groupPolicyConfiguration](../api/grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md)|Update the properties of a [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object.|
|[assign](../api/grouppolicyconfiguration-assign.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) collection||
|[updateDefinitionValues](../api/grouppolicyconfiguration-updatedefinitionvalues.md)|None||
|[List definitionValues](../api/grouppolicyconfiguration-list-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection|Get the groupPolicyDefinitionValues from the definitionValues navigation property.|
|[Add definitionValues](../api/grouppolicyconfiguration-post-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md)|Add definitionValues by posting to the definitionValues collection.|
|[List assignments](../api/grouppolicyconfiguration-list-assignments.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) collection|Get the groupPolicyConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/grouppolicyconfiguration-post-assignments.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List groupPolicyConfigurations](../api/intune-devices-devicemanagement-list-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) collection|Get the groupPolicyConfigurations from the groupPolicyConfigurations navigation property.|
|[Add groupPolicyConfigurations](../api/intune-devices-devicemanagement-post-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/grouppolicyconfiguration.md)|Add groupPolicyConfigurations by posting to the groupPolicyConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the object was created.|
|description|String|User provided description for the resource object.|
|displayName|String|User provided name for the resource object.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|roleScopeTagIds|String collection|The list of scope tags for the configuration.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) collection|The list of group assignments for the configuration.|
|definitionValues|[groupPolicyDefinitionValue](../resources/grouppolicydefinitionvalue.md) collection|The list of enabled or disabled group policy definition values for the configuration.|

## JSON Representation
Here is a JSON representation of the resource.
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

