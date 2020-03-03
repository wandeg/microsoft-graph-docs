---
title: "groupPolicyConfiguration resource type"
description: "The group policy configuration entity contains the configured values for one or more group policy definitions."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# groupPolicyConfiguration resource type

The group policy configuration entity contains the configured values for one or more group policy definitions.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyConfiguration](../api/grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/groupPolicyConfiguration.md)|Read properties and relationships of the [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object.|
|[Delete groupPolicyConfiguration](../api/grouppolicyconfiguration-delete.md)|None|Deletes a [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md).|
|[Update groupPolicyConfiguration](../api/grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/groupPolicyConfiguration.md)|Update the properties of a [groupPolicyConfiguration](../resources/grouppolicyconfiguration.md) object.|
|[assign](../api/grouppolicyconfiguration-assign.md)|[groupPolicyConfigurationAssignment](../resources/groupPolicyConfigurationAssignment.md) collection||
|[updateDefinitionValues](../api/grouppolicyconfiguration-updatedefinitionvalues.md)|None||
|[List definitionValues](../api/grouppolicyconfiguration-list-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md) collection|Get the groupPolicyDefinitionValues from the definitionValues navigation property.|
|[Add definitionValues](../api/grouppolicyconfiguration-post-definitionvalues.md)|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md)|Add definitionValues by posting to the definitionValues collection.|
|[List assignments](../api/grouppolicyconfiguration-list-assignments.md)|[groupPolicyConfigurationAssignment](../resources/groupPolicyConfigurationAssignment.md) collection|Get the groupPolicyConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/grouppolicyconfiguration-post-assignments.md)|[groupPolicyConfigurationAssignment](../resources/groupPolicyConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List groupPolicyConfigurations](../api/intune-devices-devicemanagement-list-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/groupPolicyConfiguration.md) collection|Get the groupPolicyConfigurations from the groupPolicyConfigurations navigation property.|
|[Add groupPolicyConfigurations](../api/intune-devices-devicemanagement-post-grouppolicyconfigurations.md)|[groupPolicyConfiguration](../resources/groupPolicyConfiguration.md)|Add groupPolicyConfigurations by posting to the groupPolicyConfigurations collection.|

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
|assignments|[groupPolicyConfigurationAssignment](../resources/groupPolicyConfigurationAssignment.md) collection|The list of group assignments for the configuration.|
|definitionValues|[groupPolicyDefinitionValue](../resources/groupPolicyDefinitionValue.md) collection|The list of enabled or disabled group policy definition values for the configuration.|

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

