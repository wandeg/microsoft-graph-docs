---
title: "resourceSpecificPermissionGrant resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# resourceSpecificPermissionGrant resource type


Namespace: microsoft.graph




Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List resourceSpecificPermissionGrants](../api/resourcespecificpermissiongrant-list.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|List properties and relationships of the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects.|
|[Get resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-get.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Read properties and relationships of the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[Create resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-post-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Create a new [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[Delete resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-delete.md)|None|Deletes a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md).|
|[Update resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-update.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Update the properties of a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[checkMemberGroups](../api/resourcespecificpermissiongrant-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/resourcespecificpermissiongrant-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/resourcespecificpermissiongrant-getmembergroups.md)|String collection||
|[getMemberObjects](../api/resourcespecificpermissiongrant-getmemberobjects.md)|String collection||
|[restore](../api/resourcespecificpermissiongrant-restore.md)|[directoryObject](../resources/directoryobject.md)||
|[List permissionGrants](../api/group-list-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|Get the resourceSpecificPermissionGrants from the permissionGrants navigation property.|
|[Add permissionGrants](../api/group-post-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Add permissionGrants by posting to the permissionGrants collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientAppId|String||
|clientId|String||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|permission|String||
|permissionType|String||
|resourceAppId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant",
  "baseType": "microsoft.graph.directoryObject",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "clientId": "String",
  "clientAppId": "String",
  "resourceAppId": "String",
  "permissionType": "String",
  "permission": "String"
}
```

