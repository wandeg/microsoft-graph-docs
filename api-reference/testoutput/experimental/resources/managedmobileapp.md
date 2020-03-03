---
title: "managedMobileApp resource type"
description: "The identifier for the deployment an app."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedMobileApp resource type

The identifier for the deployment an app.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedMobileApp](../api/managedmobileapp-get.md)|[managedMobileApp](../resources/managedMobileApp.md)|Read properties and relationships of the [managedMobileApp](../resources/managedmobileapp.md) object.|
|[Delete managedMobileApp](../api/managedmobileapp-delete.md)|None|Deletes a [managedMobileApp](../resources/managedmobileapp.md).|
|[Update managedMobileApp](../api/managedmobileapp-update.md)|[managedMobileApp](../resources/managedMobileApp.md)|Update the properties of a [managedMobileApp](../resources/managedmobileapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/mobileAppIdentifier.md)|The identifier for an app with it's operating system type.|
|version|String|Version of the entity.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "id": "String (identifier)",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "String"
}
```

