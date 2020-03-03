---
title: "deviceManagementEnumConstraint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementEnumConstraint resource type




Inherits from [deviceManagementConstraint](../resources/deviceManagementConstraint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|values|[deviceManagementEnumValue](../resources/deviceManagementEnumValue.md) collection|List of valid values for this string|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumConstraint",
  "values": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumValue",
      "value": "String",
      "displayName": "String"
    }
  ]
}
```

