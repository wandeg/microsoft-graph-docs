---
title: "accessPackageResourceRole resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageResourceRole resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageResource](../api/accesspackageresourcerole-list-accesspackageresource.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|Get the accessPackageResources from the accessPackageResource navigation property.|
|[Create accessPackageResource](../api/accesspackageresourcerole-post-accesspackageresource.md)|[accessPackageResource](../resources/accesspackageresource.md)|Create a new accessPackageResource object.|
|[Delete accessPackageResource](../api/accesspackageresourcerole-delete-accesspackageresource.md)|None|Delete an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Update accessPackageResource](../api/accesspackageresourcerole-update-accesspackageresource.md)|[accessPackageResource](../resources/accesspackageresource.md)|Update the properties of an accessPackageResource object.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accesspackageresource.md)|Read the properties and relationships of an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[List accessPackageResourceRoles](../api/accesspackagecatalog-list-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|Get the accessPackageResourceRoles from the accessPackageResourceRoles navigation property.|
|[Create accessPackageResourceRoles](../api/accesspackagecatalog-post-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Create a new accessPackageResourceRoles object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResource|[accessPackageResource](../resources/accesspackageresource.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

