---
title: "accessPackageResourceScope resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# accessPackageResourceScope resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accessPackageResourceScope.md)|Read properties and relationships of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Delete accessPackageResourceScope](../api/accesspackageresourcescope-delete.md)|None|Deletes a [accessPackageResourceScope](../resources/accesspackageresourcescope.md).|
|[Update accessPackageResourceScope](../api/accesspackageresourcescope-update.md)|[accessPackageResourceScope](../resources/accessPackageResourceScope.md)|Update the properties of a [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accessPackageResource.md)|Read properties and relationships of the [accessPackageResource](../resources/accesspackageresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isRootScope|Boolean||
|originId|String||
|originSystem|String||
|roleOriginId|String||
|url|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResource|[accessPackageResource](../resources/accessPackageResource.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "isRootScope": true,
  "url": "String"
}
```

