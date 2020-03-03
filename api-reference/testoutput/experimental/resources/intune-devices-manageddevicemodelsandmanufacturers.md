---
title: "managedDeviceModelsAndManufacturers resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedDeviceModelsAndManufacturers resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceManufacturers|String collection|List of Manufactures for managed devices in the account|
|deviceModels|String collection|List of Models for managed devices in the account|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```

