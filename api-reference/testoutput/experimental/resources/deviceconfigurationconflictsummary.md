---
title: "deviceConfigurationConflictSummary resource type"
description: "Conflict summary for a set of device configuration policies."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceConfigurationConflictSummary resource type

Conflict summary for a set of device configuration policies.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationConflictSummary](../api/deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/deviceConfigurationConflictSummary.md)|Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.|
|[Delete deviceConfigurationConflictSummary](../api/deviceconfigurationconflictsummary-delete.md)|None|Deletes a [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md).|
|[Update deviceConfigurationConflictSummary](../api/deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/deviceConfigurationConflictSummary.md)|Update the properties of a [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.|
|[List deviceConfigurationConflictSummary](../api/intune-devices-devicemanagement-list-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceConfigurationConflictSummary.md) collection|Get the deviceConfigurationConflictSummaries from the deviceConfigurationConflictSummary navigation property.|
|[Add deviceConfigurationConflictSummary](../api/intune-devices-devicemanagement-post-deviceconfigurationconflictsummary.md)|[deviceConfigurationConflictSummary](../resources/deviceConfigurationConflictSummary.md)|Add deviceConfigurationConflictSummary by posting to the deviceConfigurationConflictSummary collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictingDeviceConfigurations|[settingSource](../resources/settingSource.md) collection|The set of policies in conflict with the given setting|
|contributingSettings|String collection|The set of settings in conflict with the given policies|
|deviceCheckinsImpacted|Int32|The count of checkins impacted by the conflicting policies and settings|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationConflictSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "id": "String (identifier)",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource"
    }
  ],
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```

