---
title: "deviceConfigurationConflictSummary resource type"
description: "Conflict summary for a set of device configuration policies."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationConflictSummary resource type


Namespace: microsoft.graph

Conflict summary for a set of device configuration policies.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationConflictSummary](../api/deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md)|Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.|
|[Update deviceConfigurationConflictSummary](../api/deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md)|Update the properties of a [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictingDeviceConfigurations|[settingSource](../resources/settingsource.md) collection|The set of policies in conflict with the given setting|
|contributingSettings|String collection|The set of settings in conflict with the given policies|
|deviceCheckinsImpacted|Int32|The count of checkins impacted by the conflicting policies and settings|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
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

