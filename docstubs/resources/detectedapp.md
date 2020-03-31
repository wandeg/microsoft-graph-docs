---
title: "detectedApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# detectedApp resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get detectedApp](../api/detectedapp-get.md)|[detectedApp](../resources/detectedapp.md)|Read properties and relationships of the [detectedApp](../resources/detectedapp.md) object.|
|[Update detectedApp](../api/detectedapp-update.md)|[detectedApp](../resources/detectedapp.md)|Update the properties of a [detectedApp](../resources/detectedapp.md) object.|
|[List managedDevices](../api/detectedapp-list-manageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Create managedDevices](../api/detectedapp-post-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Create managedDevices by posting to the managedDevices collection.|
|[List detectedApps](../api/manageddevice-list-detectedapps.md)|[detectedApp](../resources/detectedapp.md) collection|Get the detectedApps from the detectedApps navigation property.|
|[Create detectedApps](../api/manageddevice-post-detectedapps.md)|[detectedApp](../resources/detectedapp.md)|Create detectedApps by posting to the detectedApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceCount|Int32||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|sizeInByte|Int64||
|version|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/manageddevice.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```

