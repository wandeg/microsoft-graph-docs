---
title: "accessPackageResourceScope resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageResourceScope resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Read properties and relationships of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Update accessPackageResourceScope](../api/accesspackageresourcescope-update.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Update the properties of a [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accesspackageresource.md)|Read properties and relationships of the [accessPackageResource](../resources/accesspackageresource.md) object.|

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
|accessPackageResource|[accessPackageResource](../resources/accesspackageresource.md)||

## JSON representation
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

