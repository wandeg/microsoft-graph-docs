---
title: "accessPackageResourceRole resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageResourceRole resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageResourceRoles](../api/accesspackageresourcerole-list.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|List properties and relationships of the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects.|
|[Get accessPackageResourceRole](../api/accesspackageresourcerole-get.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Read properties and relationships of the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[Create accessPackageResourceRole](../api/accesspackageresourcerole-create.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Create a new [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[Delete accessPackageResourceRole](../api/accesspackageresourcerole-delete.md)|None|Deletes a [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|[Update accessPackageResourceRole](../api/accesspackageresourcerole-update.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Update the properties of a [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accesspackageresource.md)|Read properties and relationships of the [accessPackageResource](../resources/accesspackageresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|originId|String||
|originSystem|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResource|[accessPackageResource](../resources/accesspackageresource.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRole",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "originId": "String",
  "originSystem": "String"
}
```

