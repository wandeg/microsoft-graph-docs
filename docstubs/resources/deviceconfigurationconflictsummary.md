---
title: "deviceConfigurationConflictSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationConflictSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationConflictSummary](../api/deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md)|Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.|
|[Update deviceConfigurationConflictSummary](../api/deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md)|Update the properties of a [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictingDeviceConfigurations|[settingSource](../resources/settingsource.md) collection||
|contributingSettings|String collection||
|deviceCheckinsImpacted|Int32||
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

