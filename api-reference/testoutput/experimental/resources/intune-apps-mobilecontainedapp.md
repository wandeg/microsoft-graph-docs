---
title: "mobileContainedApp resource type"
description: "An abstract class that represents a contained app in a mobileApp acting as a package."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileContainedApp resource type


Namespace: microsoft.graph

An abstract class that represents a contained app in a mobileApp acting as a package.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection|List properties and relationships of the [mobileContainedApp](../resources/mobilecontainedapp.md) objects.|
|[Get mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```

