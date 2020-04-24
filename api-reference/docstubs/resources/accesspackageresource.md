---
title: "accessPackageResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageResource resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageResources](../api/accesspackageresource-list.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|Get a list of the [accessPackageResource](../resources/accesspackageresource.md) objects and their properties.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accesspackageresource.md)|Read the properties and relationships of an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Create accessPackageResource](../api/accesspackageresource-post-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md)|Create a new [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Delete accessPackageResource](../api/accesspackageresource-delete.md)|None|Deletes an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Update accessPackageResource](../api/accesspackageresource-update.md)|[accessPackageResource](../resources/accesspackageresource.md)|Update the properties of an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[List accessPackageResourceScopes](../api/accesspackageresource-list-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection|Get the accessPackageResourceScopes from the accessPackageResourceScopes navigation property.|
|[Create accessPackageResourceScopes](../api/accesspackageresource-post-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Create a new accessPackageResourceScopes object.|
|[Delete accessPackageResourceScopes](../api/accesspackageresource-delete-accesspackageresourcescopes.md)|None|Delete an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Update accessPackageResourceScopes](../api/accesspackageresource-update-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Update the properties of an accessPackageResourceScopes object.|
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Read the properties and relationships of an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[List accessPackageResourceRoles](../api/accesspackageresource-list-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|Get the accessPackageResourceRoles from the accessPackageResourceRoles navigation property.|
|[Create accessPackageResourceRoles](../api/accesspackageresource-post-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Create a new accessPackageResourceRoles object.|
|[Delete accessPackageResourceRoles](../api/accesspackageresource-delete-accesspackageresourceroles.md)|None|Delete an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[Update accessPackageResourceRoles](../api/accesspackageresource-update-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Update the properties of an accessPackageResourceRoles object.|
|[Get accessPackageResourceRole](../api/accesspackageresourcerole-get.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Read the properties and relationships of an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addedBy|String|**TODO: Add Description**|
|addedOn|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isPendingOnboarding|Boolean|**TODO: Add Description**|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|
|resourceType|String|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResourceRoles|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|**TODO: Add Description**|
|accessPackageResourceScopes|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "url": "String",
  "resourceType": "String",
  "originId": "String",
  "originSystem": "String",
  "isPendingOnboarding": true,
  "addedBy": "String",
  "addedOn": "String (timestamp)"
}
```

