---
title: "deviceConfigurationState resource type"
description: "Device Configuration State for a given device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationState resource type


Namespace: microsoft.graph

Device Configuration State for a given device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceConfigurationStates](../api/deviceconfigurationstate-list.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|List properties and relationships of the [deviceConfigurationState](../resources/deviceconfigurationstate.md) objects.|
|[Get deviceConfigurationState](../api/deviceconfigurationstate-get.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Read properties and relationships of the [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.|
|[Create deviceConfigurationState](../api/deviceconfigurationstate-create.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Create a new [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.|
|[Delete deviceConfigurationState](../api/deviceconfigurationstate-delete.md)|None|Deletes a [deviceConfigurationState](../resources/deviceconfigurationstate.md).|
|[Update deviceConfigurationState](../api/deviceconfigurationstate-update.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Update the properties of a [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the policy for this policyBase|
|id|String| Inherited from [entity](../resources/entity.md)|
|platformType|Enumeration|Platform type that the policy applies to. Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|settingCount|Int32|Count of how many setting a policy holds|
|settingStates|[deviceConfigurationSettingState](../resources/deviceconfigurationsettingstate.md) collection||
|state|Enumeration|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|version|Int32|The version of the policy|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```

