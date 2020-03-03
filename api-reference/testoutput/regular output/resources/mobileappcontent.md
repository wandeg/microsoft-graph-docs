---
title: "mobileAppContent resource type"
description: "Contains content properties for a specific app version. Each mobileAppContent can have multiple mobileAppContentFile."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mobileAppContent resource type

Contains content properties for a specific app version. Each mobileAppContent can have multiple mobileAppContentFile.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppContent](../api/mobileappcontent-get.md)|[mobileAppContent](../resources/mobileAppContent.md)|Read properties and relationships of the [mobileAppContent](../resources/mobileappcontent.md) object.|
|[Delete mobileAppContent](../api/mobileappcontent-delete.md)|None|Deletes a [mobileAppContent](../resources/mobileappcontent.md).|
|[Update mobileAppContent](../api/mobileappcontent-update.md)|[mobileAppContent](../resources/mobileAppContent.md)|Update the properties of a [mobileAppContent](../resources/mobileappcontent.md) object.|
|[List files](../api/mobileappcontent-list-files.md)|[mobileAppContentFile](../resources/mobileAppContentFile.md) collection|Get the mobileAppContentFiles from the files navigation property.|
|[Add files](../api/mobileappcontent-post-files.md)|[mobileAppContentFile](../resources/mobileAppContentFile.md)|Add files by posting to the files collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|files|[mobileAppContentFile](../resources/mobileAppContentFile.md) collection|The list of files for this app content version.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```

