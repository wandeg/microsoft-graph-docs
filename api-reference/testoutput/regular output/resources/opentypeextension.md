---
title: "openTypeExtension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# openTypeExtension resource type


Namespace: microsoft.graph




Inherits from [extension](../resources/extension.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List openTypeExtensions](../api/opentypeextension-list.md)|[openTypeExtension](../resources/opentypeextension.md) collection|List properties and relationships of the [openTypeExtension](../resources/opentypeextension.md) objects.|
|[Get openTypeExtension](../api/opentypeextension-get.md)|[openTypeExtension](../resources/opentypeextension.md)|Read properties and relationships of the [openTypeExtension](../resources/opentypeextension.md) object.|
|[Create openTypeExtension](../api/opentypeextension-create.md)|[openTypeExtension](../resources/opentypeextension.md)|Create a new [openTypeExtension](../resources/opentypeextension.md) object.|
|[Delete openTypeExtension](../api/opentypeextension-delete.md)|None|Deletes a [openTypeExtension](../resources/opentypeextension.md).|
|[Update openTypeExtension](../api/opentypeextension-update.md)|[openTypeExtension](../resources/opentypeextension.md)|Update the properties of a [openTypeExtension](../resources/opentypeextension.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|extensionName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.openTypeExtension",
  "baseType": "microsoft.graph.extension",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.openTypeExtension",
  "id": "String (identifier)",
  "extensionName": "String"
}
```

