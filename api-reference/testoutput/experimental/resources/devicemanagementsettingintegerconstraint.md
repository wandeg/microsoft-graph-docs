---
title: "deviceManagementSettingIntegerConstraint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementSettingIntegerConstraint resource type




Inherits from [deviceManagementConstraint](../resources/deviceManagementConstraint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|maximumValue|Int32|The maximum permitted value|
|minimumValue|Int32|The minimum permitted value|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```

