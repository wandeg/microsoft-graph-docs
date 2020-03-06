---
title: "sideLoadingKey resource type"
description: "SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sideLoadingKey resource type


Namespace: microsoft.graph

SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sideLoadingKey](../api/sideloadingkey-get.md)|[sideLoadingKey](../resources/sideloadingkey.md)|Read properties and relationships of the [sideLoadingKey](../resources/sideloadingkey.md) object.|
|[Update sideLoadingKey](../api/sideloadingkey-update.md)|[sideLoadingKey](../resources/sideloadingkey.md)|Update the properties of a [sideLoadingKey](../resources/sideloadingkey.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Side Loading Key description displayed to the ITPro Admins..|
|displayName|String|Side Loading Key Name displayed to the ITPro Admins.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|String|Side Loading Key Last Updated Date displayed to the ITPro Admins.|
|totalActivation|Int32|Side Loading Key Total Activation displayed to the ITPro Admins.|
|value|String|Side Loading Key Value, it is 5x5 value, seperated by hiphens.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```

