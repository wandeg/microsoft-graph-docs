---
title: "androidDeviceComplianceLocalActionBase resource type"
description: "Local Action Configuration"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# androidDeviceComplianceLocalActionBase resource type

Local Action Configuration


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidDeviceComplianceLocalActionBases](../api/androiddevicecompliancelocalactionbase-list.md)|[androidDeviceComplianceLocalActionBase](../resources/androidDeviceComplianceLocalActionBase.md) collection|List properties and relationships of the [androidDeviceComplianceLocalActionBase](../resources/androiddevicecompliancelocalactionbase.md) objects.|
|[Get androidDeviceComplianceLocalActionBase](../api/androiddevicecompliancelocalactionbase-get.md)|[androidDeviceComplianceLocalActionBase](../resources/androidDeviceComplianceLocalActionBase.md)|Read properties and relationships of the [androidDeviceComplianceLocalActionBase](../resources/androiddevicecompliancelocalactionbase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|Number of minutes to wait till a local action is enforced. Valid values 0 to 2147483647|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceComplianceLocalActionBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceComplianceLocalActionBase",
  "id": "String (identifier)",
  "gracePeriodInMinutes": 1024
}
```

