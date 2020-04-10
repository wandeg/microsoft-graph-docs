---
title: "accessPackageResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageResource resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageResources](../api/accesspackageresource-list.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|List properties and relationships of the [accessPackageResource](../resources/accesspackageresource.md) objects.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accesspackageresource.md)|Read properties and relationships of the [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Create accessPackageResource](../api/accesspackageresource-post-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md)|Create a new [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Delete accessPackageResource](../api/accesspackageresource-delete.md)|None|Deletes a [accessPackageResource](../resources/accesspackageresource.md).|
|[Update accessPackageResource](../api/accesspackageresource-update.md)|[accessPackageResource](../resources/accesspackageresource.md)|Update the properties of a [accessPackageResource](../resources/accesspackageresource.md) object.|
|[List accessPackageResourceScopes](../api/accesspackageresource-list-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection|Get the accessPackageResourceScopes from the accessPackageResourceScopes navigation property.|
|[Add accessPackageResourceScopes](../api/accesspackageresource-post-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Add accessPackageResourceScopes by posting to the accessPackageResourceScopes collection.|
|[List accessPackageResourceRoles](../api/accesspackageresource-list-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|Get the accessPackageResourceRoles from the accessPackageResourceRoles navigation property.|
|[Add accessPackageResourceRoles](../api/accesspackageresource-post-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Add accessPackageResourceRoles by posting to the accessPackageResourceRoles collection.|
|[List accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|Get the accessPackageResources from the accessPackageResources navigation property.|
|[Add accessPackageResources](../api/accesspackagecatalog-post-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md)|Add accessPackageResources by posting to the accessPackageResources collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addedBy|String||
|addedOn|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isPendingOnboarding|Boolean||
|originId|String||
|originSystem|String||
|resourceType|String||
|url|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResourceRoles|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection||
|accessPackageResourceScopes|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection||

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

