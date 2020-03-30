---
title: "deviceManagementEnumConstraint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementEnumConstraint resource type


Namespace: microsoft.graph




Inherits from [deviceManagementConstraint](../resources/devicemanagementconstraint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|values|[deviceManagementEnumValue](../resources/devicemanagementenumvalue.md) collection||

## Relationships
None

## JSON representation
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

