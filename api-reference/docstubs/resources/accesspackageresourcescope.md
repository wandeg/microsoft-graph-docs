---
title: "accessPackageResourceScope resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageResourceScope resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Read the properties and relationships of an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Update accessPackageResourceScope](../api/accesspackageresourcescope-update.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Update the properties of an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[List accessPackageResource](../api/accesspackageresourcescope-list-accesspackageresource.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|Get the accessPackageResources from the accessPackageResource navigation property.|
|[Create accessPackageResource](../api/accesspackageresourcescope-post-accesspackageresource.md)|[accessPackageResource](../resources/accesspackageresource.md)|Create a new accessPackageResource object.|
|[Delete accessPackageResource](../api/accesspackageresourcescope-delete-accesspackageresource.md)|None|Delete an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Update accessPackageResource](../api/accesspackageresourcescope-update-accesspackageresource.md)|[accessPackageResource](../resources/accesspackageresource.md)|Update the properties of an accessPackageResource object.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accesspackageresource.md)|Read the properties and relationships of an [accessPackageResource](../resources/accesspackageresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isRootScope|Boolean|**TODO: Add Description**|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|
|roleOriginId|String|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResource|[accessPackageResource](../resources/accesspackageresource.md)|**TODO: Add Description**|

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

