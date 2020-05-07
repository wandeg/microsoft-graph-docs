---
title: "managedDeviceModelsAndManufacturers resource type"
description: "Models and Manufactures meatadata for managed devices in the account"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceModelsAndManufacturers resource type


Namespace: microsoft.graph

Models and Manufactures meatadata for managed devices in the account

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceManufacturers|String collection|List of Manufactures for managed devices in the account|
|deviceModels|String collection|List of Models for managed devices in the account|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```

