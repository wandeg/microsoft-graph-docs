---
title: "resourceSpecificPermissionGrant resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# resourceSpecificPermissionGrant resource type

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryObject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List resourceSpecificPermissionGrants](../api/resourcespecificpermissiongrant-list.md)|[resourceSpecificPermissionGrant](../resources/resourceSpecificPermissionGrant.md) collection|List properties and relationships of the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects.|
|[Get resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-get.md)|[resourceSpecificPermissionGrant](../resources/resourceSpecificPermissionGrant.md)|Read properties and relationships of the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[Create resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-post-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourceSpecificPermissionGrant.md)|Create a new [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[Delete resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-delete.md)|None|Deletes a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md).|
|[Update resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-update.md)|[resourceSpecificPermissionGrant](../resources/resourceSpecificPermissionGrant.md)|Update the properties of a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[checkMemberGroups](../api/resourcespecificpermissiongrant-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/resourcespecificpermissiongrant-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/resourcespecificpermissiongrant-getmembergroups.md)|String collection||
|[getMemberObjects](../api/resourcespecificpermissiongrant-getmemberobjects.md)|String collection||
|[restore](../api/resourcespecificpermissiongrant-restore.md)|[directoryObject](../resources/directoryObject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientAppId|String||
|clientId|String||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|permission|String||
|permissionType|String||
|resourceAppId|String||

## Relationships
None

## JSON Representation
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

