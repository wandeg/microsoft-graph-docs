---
title: "deviceSetupConfiguration resource type"
description: "This is the base class for Setup Configuration. Setup configurations are platform specific and individual per-platform setup configurations inherit from here."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceSetupConfiguration resource type


Namespace: microsoft.graph

This is the base class for Setup Configuration. Setup configurations are platform specific and individual per-platform setup configurations inherit from here.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceSetupConfigurations](../api/devicesetupconfiguration-list.md)|[deviceSetupConfiguration](../resources/devicesetupconfiguration.md) collection|List properties and relationships of the [deviceSetupConfiguration](../resources/devicesetupconfiguration.md) objects.|
|[Get deviceSetupConfiguration](../api/devicesetupconfiguration-get.md)|[deviceSetupConfiguration](../resources/devicesetupconfiguration.md)|Read properties and relationships of the [deviceSetupConfiguration](../resources/devicesetupconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|displayName|String|Admin provided name of the device configuration.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|version|Int32|Version of the device configuration.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceSetupConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceSetupConfiguration",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```

