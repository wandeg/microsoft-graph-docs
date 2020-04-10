---
title: "printIdentity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printIdentity resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printIdentity](../api/printidentity-get.md)|[printIdentity](../resources/printidentity.md)|Read properties and relationships of the [printIdentity](../resources/printidentity.md) object.|
|[Update printIdentity](../api/printidentity-update.md)|[printIdentity](../resources/printidentity.md)|Update the properties of a [printIdentity](../resources/printidentity.md) object.|
|[List allowedGroups](../api/printer-list-allowedgroups.md)|[printIdentity](../resources/printidentity.md) collection|Get the printIdentities from the allowedGroups navigation property.|
|[Add allowedGroups](../api/printer-post-allowedgroups.md)|[printIdentity](../resources/printidentity.md)|Add allowedGroups by posting to the allowedGroups collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printIdentity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printIdentity",
  "id": "String (identifier)",
  "displayName": "String"
}
```

