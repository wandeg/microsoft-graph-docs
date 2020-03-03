---
title: "workbookFormatProtection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookFormatProtection resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookFormatProtections](../api/workbookformatprotection-list.md)|[workbookFormatProtection](../resources/workbookFormatProtection.md) collection|List properties and relationships of the [workbookFormatProtection](../resources/workbookformatprotection.md) objects.|
|[Get workbookFormatProtection](../api/workbookformatprotection-get.md)|[workbookFormatProtection](../resources/workbookFormatProtection.md)|Read properties and relationships of the [workbookFormatProtection](../resources/workbookformatprotection.md) object.|
|[Create workbookFormatProtection](../api/workbookformatprotection-create.md)|[workbookFormatProtection](../resources/workbookFormatProtection.md)|Create a new [workbookFormatProtection](../resources/workbookformatprotection.md) object.|
|[Delete workbookFormatProtection](../api/workbookformatprotection-delete.md)|None|Deletes a [workbookFormatProtection](../resources/workbookformatprotection.md).|
|[Update workbookFormatProtection](../api/workbookformatprotection-update.md)|[workbookFormatProtection](../resources/workbookFormatProtection.md)|Update the properties of a [workbookFormatProtection](../resources/workbookformatprotection.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|formulaHidden|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|locked|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookFormatProtection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookFormatProtection",
  "id": "String (identifier)",
  "formulaHidden": true,
  "locked": true
}
```

